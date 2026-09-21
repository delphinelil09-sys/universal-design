# Install

The five skills live in the repository at:

- `design-core/` — the entry point (SKILL.md + 6 references)
- `design-promo/` — landing page lens
- `design-portfolio/` — portfolio lens
- `design-ecommerce/` — ecommerce lens
- `design-info/` — info site lens

## Get the files (git)

```bash
git clone <your-repo-url>
cd <repo>
```

or download the repository as a ZIP and unpack it.

## Target location (Chatbox)

Copy the five skill directories into the Chatbox global skills folder.

Standard locations by OS:

| OS | Skills folder |
|---|---|
| Windows | `C:\Users\<USER>\AppData\Roaming\xyz.chatboxapp.app\skills\` |
| macOS | `~/Library/Application Support/xyz.chatboxapp.app/skills/` |
| Linux | `~/.config/xyz.chatboxapp.app/skills/` |

> macOS/Linux paths follow the standard Electron convention; create the `skills` folder if it doesn't exist. (Confirmed on Windows.)

Windows copy command (PowerShell):

```powershell
$dest = "$env:APPDATA\xyz.chatboxapp.app\skills"
$xcopy 'design-core' (Join-Path $dest 'design-core') /E /I
$xcopy 'design-promo' (Join-Path $dest 'design-promo') /E /I
$xcopy 'design-portfolio' (Join-Path $dest 'design-portfolio') /E /I
$xcopy 'design-ecommerce' (Join-Path $dest 'design-ecommerce') /E /I
$xcopy 'design-info' (Join-Path $dest 'design-info') /E /I
```

macOS/Linux copy command:

```bash
SKILLS_DIR=~"/Library/Application Support/xyz.chatboxapp.app/skills"  # macOS
# SKILLS_DIR=~/.config/xyz.chatboxapp.app/skills                      # Linux
mkdir -p "$SKILLS_DIR"
cp -r design-core design-promo design-portfolio design-ecommerce design-info "$SKILLS_DIR/"
```

Result:

```
skills/
├── design-core/
│   ├── SKILL.md
│   └── references/
│       ├── elements.md
│       ├── layers.md
│       ├── audit-grid.md
│       ├── generation.md
│       ├── marketing.md
│       └── trends-2026-Q3.md
├── design-promo/SKILL.md
├── design-portfolio/SKILL.md
├── design-ecommerce/SKILL.md
└── design-info/SKILL.md
```

Do **not** copy `_evals/` — it is dev tooling, not a skill (no top-level SKILL.md).

## Order matters

`design-core` must appear **before** the four subtype skills in any listing the model sees. Its description is written to trigger on generic design requests ("make my site look better", "why does it look generic"). The subtypes are written to trigger more narrowly. If a subtype appears first, a generic request may route directly to a subtype and skip the three entry steps.

In the Chatbox skills folder the directories sort alphabetically, and `design-core` sorts before `design-{ecommerce,info,portfolio,promo}` — the required order holds by name.

## Verifying the trigger

After install, restart Chatbox, start a fresh session and paste: *"Here's my site — can you make it better?"* The `design-core` skill should trigger, not a subtype.

Then paste: *"I need a portfolio site for a photographer."* The `design-portfolio` skill may trigger directly — that's fine, as long as it defers to `design-core` for the method.

## Chatbox environment notes

- No packaging step is needed: Chatbox loads skills directly from directories.
- No git step inside the skills folder is needed: the folder is not a repository.
- Sub-skill loading is manual (reference files are read on demand), which matches the "load on demand" design of the references.
- Requires the Chatbox desktop app with agent-mode support and a tool-capable model.