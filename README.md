<div align="center">

# Frontend UI Pro

### Scan. Explore. Design. Improve.

**A reusable AI skill for frontend UI analysis, design discovery, design-system import, color palettes, and implementation guidance.**

[![Skill](https://img.shields.io/badge/AI-Skill-6C5CE7?style=for-the-badge)](#)
[![Markdown](https://img.shields.io/badge/Docs-Markdown-111827?style=for-the-badge&logo=markdown&logoColor=white)](#)
[![UI Types](https://img.shields.io/badge/UI_Catalog-150_Types-0891B2?style=for-the-badge)](ui-types.md)
[![License: MIT](https://img.shields.io/badge/License-MIT-16A34A?style=for-the-badge)](LICENSE)

**Give your AI coding agent a structured workflow for understanding and improving frontend interfaces.**

</div>

---

## Contents

- [What is Frontend UI Pro?](#what-is-frontend-ui-pro)
- [Features](#features)
- [Repository files](#repository-files)
- [Installation](#installation)
- [How to use it](#how-to-use-it)
- [Slash-command examples](#slash-command-examples)
- [Import a design specification](#import-a-design-specification)
- [Import or create a color palette](#import-or-create-a-color-palette)
- [Recommended workflow](#recommended-workflow)
- [Compatibility and limitations](#compatibility-and-limitations)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## What is Frontend UI Pro?

Frontend UI Pro is a Markdown-based skill for AI coding agents. It provides a repeatable workflow for inspecting a frontend project, exploring design directions, using design references, mapping color palettes, and planning or implementing UI improvements.

It is designed to work with an existing project instead of assuming every project should be rebuilt from scratch.

> **Important:** Frontend UI Pro is a set of instructions and reference documents. It is not a standalone visual editor or website preview application.

## Features

- **Existing UI review** — inspect available project files and identify layout, typography, spacing, component, accessibility, and responsive-design opportunities.
- **Design suggestions** — recommend a short list of suitable UI directions based on the project and its audience.
- **UI type catalog** — browse 150 practical UI styles, page types, layouts, and interaction patterns.
- **Design specification support** — use a local `design.md`, pasted design rules, or a reachable GitHub file URL as a design reference.
- **Color palette support** — map HEX colors to semantic tokens or generate a starter palette.
- **Implementation planning** — propose focused changes while preserving existing functionality.
- **Responsive and accessibility guidance** — consider mobile layouts, keyboard access, focus states, contrast, and meaningful component states.
- **Reference files** — keep detailed guidance in separate Markdown files so the main skill stays readable.

## Repository files

| File | Purpose |
|---|---|
| `SKILL.md` | Main instructions and workflow for the AI agent |
| `design.md` | Design-system specification template |
| `ui-types.md` | Catalog of 150 UI styles, page types, layouts, and patterns |
| `color-palettes.md` | Semantic color roles, example palettes, and accessibility guidance |
| `design-examples.md` | Written design examples and reusable UI patterns |
| `README.md` | Project overview, setup, and usage guide |

Keep the reference files alongside `SKILL.md` so the agent can follow its relative references.

## Installation

### Option A — Install from this repository

1. Open this repository on GitHub.
2. Download the repository as a ZIP, or clone it:
   ```bash
   git clone https://github.com/YOUR-USERNAME/frontend-ui-pro.git
   ```
3. Extract or clone the files.
4. Find the skill installation instructions for your specific AI coding agent.
5. Copy the complete skill folder, including `SKILL.md` and its reference files, into the agent's supported skills directory.
6. If the agent requires a particular folder structure or metadata format, follow its official instructions.
7. Restart or reload the agent if required.
8. Open a frontend project and ask the agent to use **Frontend UI Pro**.
9. Test it with a scan request before asking it to edit code.

Replace `YOUR-USERNAME` with the GitHub account or organization that owns the repository.

### Option B — Add it manually

1. Create a folder named `frontend-ui-pro` in the skills directory supported by your AI coding agent.
2. Place all six Markdown files inside that folder.
3. Check that `SKILL.md` includes the required metadata for your agent.
4. Confirm that the agent can read the reference files.
5. Reload the agent if necessary and run a test prompt.

**There is no single universal skills folder for every AI tool.** Some agents use different folder paths, metadata, or installation mechanisms. Use the folder documented by your chosen agent rather than assuming a particular drive or path.

## How to use it

Once the skill is installed and recognized by your AI coding agent, open the project you want to work on and try one of these prompts.

### 1. Scan the existing UI

```text
Use Frontend UI Pro to scan this frontend project.
Identify the current framework, page structure, styling approach,
UI inconsistencies, responsive issues, and accessibility opportunities.
Recommend 3 to 5 suitable design directions.
Do not modify files yet.
```

The agent should inspect the project files it can access and report evidence-based findings. Visual behavior that cannot be verified from source files should be labeled as unverified.

### 2. Explore UI styles

```text
Use Frontend UI Pro to show me suitable UI styles for this project.
Explain the best options, why each fits, its visual characteristics,
relevant components, responsive behavior, and trade-offs.
```

You can also ask about a specific style, such as Glassmorphism, Bento Grid, Minimalist UI, or Dark Developer Dashboard. See [`ui-types.md`](ui-types.md).

### 3. Select a design direction

```text
Use Frontend UI Pro.
I choose the Bento Grid style for the feature section.
Create an implementation plan that fits the existing framework
and preserves current functionality. Wait for my approval before editing.
```

### 4. Import a design specification

```text
Use Frontend UI Pro to read my design specification:
https://github.com/YOUR-USERNAME/YOUR-REPO/blob/main/design.md

If you can access the file, summarize its design tokens and rules.
If you cannot access it, ask me to paste the file contents.
Do not claim the file was imported unless you actually read it.
```

Replace the example URL with your actual file URL. A raw GitHub file URL may be easier for some tools to retrieve. You can also paste the contents of `design.md` directly into the conversation.

### 5. Create or import a color palette

```text
Use Frontend UI Pro to create a modern color palette for this project.
Provide HEX values for primary, secondary, background, surface, text,
muted text, border, accent, success, warning, and error.
Consider light and dark themes and check contrast when tools are available.
```

For palette guidance and starter examples, see [`color-palettes.md`](color-palettes.md).

### 6. Implement the approved design

```text
Use Frontend UI Pro to implement the approved design plan.
Reuse existing components where appropriate, keep the current framework,
preserve routes and functionality, make the layout responsive, and avoid
unnecessary dependencies. Run available checks and summarize changed files.
```

Implementation requires the agent to have access to your project and permission to edit files.

## Slash-command examples

The following are suggested command patterns for agents that support custom slash commands or skill invocation:

| Command pattern | Intended action |
|---|---|
| `/ui-design scan` | Review the existing UI |
| `/ui-design suggest` | Recommend design directions |
| `/ui-design types glassmorphism` | Explore a UI type |
| `/ui-design import-design URL` | Read a design specification |
| `/ui-design colors` | Import or create a color palette |
| `/ui-design generate` | Plan or implement an approved design |
| `/ui-design review` | Review the implementation |
| `/ui-design responsive` | Inspect responsive behavior |

**Slash-command note:** Writing these patterns in Markdown does not automatically register them. Your AI coding agent must support and register the relevant command or skill invocation. If it does not, use the same text as a normal prompt.

## Import a design specification

Use `design.md` as a shared design-system reference. It includes sections for:

- Design goals and audience
- Color tokens
- Typography and spacing
- Shape, elevation, and layout
- Component styles and states
- Motion
- Responsive behavior
- Accessibility
- Implementation notes

You can keep your own specification in the repository, provide its contents directly, or ask the agent to retrieve an accessible URL. Always verify that the agent successfully read the intended file.

## Import or create a color palette

A useful palette describes the purpose of each color rather than only listing swatches.

Common semantic roles include:

- `primary` — main actions and links
- `secondary` — supporting actions
- `background` — page background
- `surface` — cards, panels, and menus
- `text` — primary text
- `muted` — secondary text
- `border` — outlines and dividers
- `accent` — visual emphasis
- `success`, `warning`, and `error` — status feedback

Provide HEX values, a palette file, or a URL the agent can access. Ask for light and dark variants if needed. Color contrast should be checked with a reliable tool when available; untested contrast should not be described as verified.

## Recommended workflow

1. **Inspect** — understand the existing code and UI.
2. **Recommend** — compare a small set of relevant design directions.
3. **Choose** — select the style and constraints.
4. **Import** — provide design rules and color tokens if you have them.
5. **Plan** — review the proposed changes before implementation.
6. **Implement** — update the relevant components without unnecessary rewrites.
7. **Verify** — run available tests and review responsive behavior and accessibility.
8. **Summarize** — list changed files, checks performed, and known limitations.

This workflow helps avoid unrequested redesigns and reduces the risk of breaking existing features.

## Compatibility and limitations

- The skill depends on the capabilities and configuration of the AI coding agent.
- Different agents may require different skill directory paths or metadata.
- URL import requires network or connector access to the requested file.
- UI scanning can only inspect files and runtime behavior available to the agent.
- Visual previews require a browser, screenshot, or preview tool.
- Editing requires appropriate project access and permissions.
- A skill alone does not create a graphical menu or guarantee that a custom slash command exists.
- Design suggestions are guidance, not a guarantee of better usability; review and test changes with real users where possible.

## Troubleshooting

**The agent does not recognize the skill**
- Confirm that the files are in the agent's documented skills directory.
- Confirm the folder contains `SKILL.md` and all referenced Markdown files.
- Check required metadata and reload the agent if necessary.

**The `/ui-design` command does not work**
- Confirm that the agent supports custom slash commands and that the command is registered.
- Otherwise, use a normal prompt such as: `Use Frontend UI Pro to scan this project.`

**A design URL cannot be imported**
- Check that the URL is accessible to the agent.
- Try a raw file URL if supported.
- Paste the Markdown contents directly if retrieval still fails.

**The agent suggests changes without understanding the project**
- Ask it to inspect the relevant page, components, styles, and package configuration first.
- Request that it separate verified findings from assumptions.
- Ask for a plan before allowing edits.

## Contributing

Contributions are welcome. When adding a UI type or design example:

1. Explain what it is and when it is useful.
2. Include visual characteristics and relevant components.
3. Describe responsive and accessibility considerations.
4. Mention trade-offs or performance concerns.
5. Avoid duplicate entries added only to increase the catalog size.

## License

This project is distributed under the MIT License. See [`LICENSE`](LICENSE) for the license text.

---

<div align="center">

**Frontend UI Pro — a structured starting point for better frontend design workflows.**

If this project is useful, consider starring the repository and sharing feedback or improvements.

</div>
