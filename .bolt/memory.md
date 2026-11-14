# Project memory

## Product intent & audience

- YouTubeDownloader: a desktop application for downloading YouTube videos.
- Primary surface is a native desktop window; not designed as a web app.
- Audience: end users running the app locally on a desktop computer.

## Brand personality & voice

- Practical, utility-focused tool. No strong consumer-brand framing inferred yet.
- Documentation tone is straightforward and feature-oriented.

## Visual design & UX direction

- App UI includes a header, a URL input box, and a feature list.
- Three screenshots exist in the project and represent the real app UI.
- Web preview is a static stand-in page (Vite + index.html at root) that mirrors these elements; it is not interactive.
- No inferred design system, color tokens, or typography choices yet.

## Decisions, constraints & rationale

- Project root originally had no web setup (no package.json / index.html), causing preview failure.
- Added a minimal Vite web preview at root so Bolt preview can render something; rationale: the real app is desktop-only and cannot run in a browser preview.
- Build output was cleaned so only source files remain.
- A fully interactive web version would require a web rebuild of the app — intentionally out of scope for the preview fix.

## Open questions & assumptions

- Assumption: the three screenshots and README feature list accurately represent the current app UI.
- Unverified whether the preview actually loads for the user (assistant could not self-check).
- Unknown: desired tech stack for the real desktop app (e.g., Electron, .NET, other).
- Unknown: whether a full web port of the app is wanted in the future.