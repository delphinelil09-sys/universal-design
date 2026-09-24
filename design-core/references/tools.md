# Tools

Rules for editing files safely. Load this when the task involves writing or modifying files, not only when designing.

## Line endings (CRLF)

Files created on Windows often use CRLF (`\r\n`) instead of LF (`\n`). Multi-line `old_text` written with `\n` will silently fail to match against a CRLF file.

Before editing any file on Windows:

1. Check line endings. PowerShell:

```powershell
$c = Get-Content -Raw 'path\to\file'; [bool]($c -match "\r\n")
```

2. If `True` — the file is CRLF. Either convert it to LF, or use `\r\n` in `old_text`.

Convert to LF (string overload, not char — PowerShell 5.1 has no char overload for `Replace`):

```powershell
$c = Get-Content -Raw 'path\to\file'
$c = $c.Replace("`r`n", "`n")
Set-Content -NoNewline -Encoding UTF8 'path\to\file' $c
```

Do not use `[char]13 + [char]10` — the char overload does not exist in Windows PowerShell 5.1 and fails silently.

## Batch limits

Do not make all edits to a large file in one call. If one edit in a batch fails to match, the entire batch is rejected — you lose everything in it.

Default batch size: **10 edits**.

Reduce to **5** when:
- The file is over 1000 lines.
- Edits touch JS logic, CSS animations, or anything stateful.
- Edits are multi-line blocks (more than 3 lines of `old_text`).

Increase to **15–20** when:
- The file is under 300 lines.
- All edits are single-line string replacements.
- The same edit pattern has already been verified on this file.

After each batch: verify. Read one or two control lines to confirm the change landed. Do not re-read the whole file.

If a batch fails: **halve the size** and retry. Do not repeat the same failing batch.

## Scope discipline for edits

Edit exactly what was asked. Nothing else.

If you notice something else worth fixing during an edit — do not touch it. Note it in the report. The user decides whether to address it.

Why: scope creep makes the change unpredictable. The user asked for one fix; if they get three, they have to review two they did not anticipate. This breaks trust.

This applies to:
- Cosmetic issues (typos, formatting, inconsistency).
- Structural issues (missing files, broken links).
- Anything outside the stated task.

Report it. Do not fix it.