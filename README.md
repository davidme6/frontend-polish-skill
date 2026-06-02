# Frontend Polish Skill

Frontend Polish is a Codex skill for turning rough, generic, or AI-generated frontend work into product-grade UI without rewriting the underlying business logic.

It gives Codex a repeatable design-engineering workflow for improving hierarchy, spacing, typography, responsiveness, interaction states, and implementation quality across React, Vue, Tailwind CSS, and plain HTML/CSS projects.

## Why This Skill Exists

AI-generated interfaces often work, but they can still feel unfinished:

- every section looks like the same card
- gradients and shadows are used as decoration instead of emphasis
- desktop layouts collapse awkwardly on mobile
- hover, focus, disabled, loading, and error states are thin or missing
- dashboards become too airy, while landing pages feel templated
- the code gets harder to maintain after visual changes

This skill helps Codex polish the frontend like a senior frontend engineer and UI design engineer: preserve the product intent, keep the existing stack, and improve the interface where it matters most.

## What It Helps With

- UI polish for existing pages and components
- Reducing the "AI template" feel in generated frontends
- Responsive layout cleanup for mobile and desktop
- Better visual hierarchy, grouping, density, and scan paths
- More intentional color, typography, spacing, borders, and shadows
- Production-quality interaction states
- Component-level refinement without full redesigns
- Dashboard and internal-tool polish that stays dense and useful
- Landing page, auth page, product detail page, and ecommerce refinement
- Frontend cleanup that respects the existing codebase

## Common Use Cases

### Landing Pages

Use it when a marketing page technically works but feels generic. The skill focuses on message hierarchy, section rhythm, CTA emphasis, mobile composition, and avoiding overused SaaS visual patterns.

### Dashboards And Admin Tools

Use it when a dashboard needs to feel clearer and more professional without turning into a marketing site. The skill prioritizes grouping, table rhythm, filters, status colors, density, and repeat-use ergonomics.

### Auth Flows

Use it for sign-in, sign-up, reset password, invitation, and onboarding screens. The skill makes forms calmer, more trustworthy, and easier to scan while preserving fields and validation logic.

### Components

Use it for buttons, cards, forms, tables, modals, nav, data display, and reusable UI primitives. The skill focuses on states, spacing, hierarchy, API compatibility, and maintainability.

### AI-Generated Prototypes

Use it after a first pass from Codex, Claude, v0, Bolt, Lovable, Cursor, or another generator. It is especially useful when the app has the right functionality but the UI still looks repetitive or machine-made.

## Install

Clone this repository and copy the skill folder into your Codex skills directory:

```bash
git clone https://github.com/davidme6/frontend-polish-skill.git
mkdir -p ~/.codex/skills
cp -R frontend-polish-skill/skills/frontend-polish ~/.codex/skills/frontend-polish
```

On Windows PowerShell:

```powershell
git clone https://github.com/davidme6/frontend-polish-skill.git
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\skills" | Out-Null
Copy-Item -Recurse -Force "frontend-polish-skill\skills\frontend-polish" "$env:USERPROFILE\.codex\skills\frontend-polish"
```

If you use a Codex marketplace installer that supports GitHub skill paths:

```bash
npx codex-marketplace add davidme6/frontend-polish-skill/skills/frontend-polish
```

## Example Prompts

```text
Use $frontend-polish to refine this page so it feels less AI-generated and more product-grade. Keep the logic intact and edit the code directly.
```

```text
Use $frontend-polish to polish this dashboard without turning it into a marketing page. Keep the data flow and filters unchanged. Focus on grouping, table rhythm, filter clarity, status color discipline, and responsive behavior.
```

```text
Use $frontend-polish to improve this sign-in page. Keep the form fields and validation logic unchanged. Make it feel calmer, more trustworthy, and more intentional on mobile.
```

```text
Use $frontend-polish to polish this component only. Do not redesign the whole page. Focus on spacing, visual hierarchy, hover/focus/disabled/loading states, and implementation cleanliness.
```

## Skill Structure

```text
skills/frontend-polish/
  SKILL.md
  agents/openai.yaml
  references/
    call-examples.md
    polish-playbook.md
```

- `SKILL.md` contains the core operating instructions and trigger metadata.
- `agents/openai.yaml` contains UI metadata for Codex skill lists.
- `references/polish-playbook.md` provides deeper design and code review guidance.
- `references/call-examples.md` provides reusable prompts for different frontend situations.

## Design Philosophy

Frontend Polish is intentionally restrained. It does not tell Codex to add visual spectacle everywhere. It tells Codex to make better product decisions:

- structure before decoration
- hierarchy before effects
- states before screenshots
- mobile composition before breakpoint recipes
- maintainability before visual tricks
- product context before trend chasing

The goal is not to make every interface look expensive. The goal is to make each interface feel intentional, useful, and believable in a real product.

## Contributing

Issues, examples, pull requests, and before/after screenshots are very welcome. Useful feedback includes:

- prompts where the skill triggered too often or not often enough
- UI polish tasks where the guidance felt too vague
- framework-specific patterns for React, Vue, Tailwind, or plain CSS
- screenshots showing recurring "AI-generated" frontend problems
- better examples for dashboards, auth flows, ecommerce, or component systems

Please keep the skill itself concise. Long explanations and examples usually belong in `references/`, not in `SKILL.md`.

## License

MIT. See [LICENSE](LICENSE).
