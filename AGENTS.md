# Project instructions — African Netflix

These instructions apply to all work in this repository. The active working branch for the current player work is `fix/season-selector-bubble`. Never push these changes to `main` or promote a preview to production unless the user explicitly approves.

## Project-specific priorities

1. Preserve existing working screens and interactions. Make surgical changes only.
2. Treat the user's screenshots and explicit layout instructions as the source of truth. Do not redesign unrelated screens.
3. For the player, preserve the requested full-screen landscape composition: episode title at top-left; reactions at top-centre; cast, picture-in-picture, minimise and lock at top-right; playback controls centred; brightness left and volume right; timeline and action toolbar at the bottom; compact horizontal episode thumbnails when Episodes is opened.
4. Do not add a portrait “turn your phone sideways” screen. Attempt native orientation only where supported; never claim iOS Safari can be forced into landscape if it cannot.
5. Do not claim video playback, casting, clipping, subtitles or other media features work until real media sources/services are connected and tested.
6. Keep the user's existing Season button placement and appearance unchanged unless explicitly asked.
7. Use the project's existing HTML/CSS/JavaScript and Lucide icon approach. Do not introduce a framework or dependency without a clear need.
8. Verify at phone and desktop sizes. When visual accuracy matters, inspect a real rendered preview; source/HTML checks alone do not prove visual correctness.
9. Run relevant checks and report what was actually tested, what failed, and what remains unverified.
10. Keep edits on the current feature branch. Never touch production/main without explicit approval.

## Skills to apply

Use these upstream Agent Skills as review and implementation guidance. Read the linked skill's `SKILL.md` and any references it explicitly requires before relying on its detailed rules. Do not pretend a skill is installed locally when only its upstream source is linked.

### Core UI work — apply on every player, screen or interaction change

- **UI UX Pro Max** — https://github.com/nextlevelbuilder/ui-ux-pro-max-skill  
  Use for design-system consistency, mobile-first layout, touch targets, accessibility, performance, typography, contrast and responsive behavior.
- **Taste Skill** — https://github.com/Leonxlnx/taste-skill  
  Use to avoid generic/template-like design. Preserve a coherent visual voice, deliberate composition, restrained motion and high-quality finish. Adapt its website-specific rules to this streaming interface; do not blindly impose landing-page section rules on a media player.
- **Hallmark** — https://github.com/Nutlope/hallmark  
  Use for visual direction, distinctive material/theme choices, content-first composition and anti-generic design checks. Do not redesign a screen when the request is a narrow fix.
- **Interface Skills** — https://github.com/jakubkrehel/skills  
  Apply the relevant skills from this collection: `better-interface`, `better-accessibility`, `better-layout`, `better-writing`, `better-typography`, `better-colors`, `better-ui`, and `better-motion`. Use `interface-review` for user-requested change reviews; do not claim to have run it if unavailable.

### Use when the task calls for them

- **Stitch Skills** — https://github.com/google-labs-code/stitch-skills  
  Use design-generation or code-to-design workflows when a new visual direction or design handoff is requested. Stitch MCP credentials/service are prerequisites; do not assume they exist.
- **Website Cloner** — https://github.com/JCodesMore/ai-website-cloner-template  
  Use only when the user asks to study or recreate a reference website. Inspect the reference and distinguish copied structure from original project requirements. Do not clone protected assets or branding.
- **Diagram Design** — https://github.com/cathrynlavery/diagram-design  
  Use for architecture, state-flow, playback-flow or system diagrams when requested or when they materially clarify a technical change. Not a substitute for implementing or testing behavior.
- **Frontend Slides** — https://github.com/zarazhangrui/frontend-slides  
  Use only for HTML presentations/decks requested by the user. It is not a routine website/player design skill.
- **Scroll World** — https://github.com/oso95/scroll-world  
  Use only when the user explicitly requests a cinematic scroll-driven landing page. Its external rendering tools may incur costs; obtain approval before any paid generation.

### Unresolved repository reference

- **Archify** — user supplied `tt-ali/archify`, but the repository could not be located/verified during setup. Do not invent its contents or claim it is installed. Retry only when its correct public repository URL or access is available.

## How to resolve conflicting guidance

The user's explicit request and project-specific constraints take priority. Then preserve existing architecture and behavior. Apply relevant skill guidance where it improves the requested work. If two skills conflict, state the trade-off and choose the least disruptive option. Never let a skill silently authorize unrelated redesign, dependency changes, paid services, production deployment or destructive actions.

## Required delivery note

For each substantial UI change, report:
- files and screens changed;
- the applicable skills/guidance used;
- checks actually run and their results;
- visual/runtime behavior not verified;
- preview URL and branch, when available.
