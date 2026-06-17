# terminal-portfolio — AI/ML Engineer

A command-line style portfolio in a single, dependency-free `index.html`
(vanilla HTML + CSS + JS). Boots like a machine loading model weights,
then drops the visitor into an interactive shell.

## Quick start
Open `index.html` in any browser. That's it — no build step, no server needed.

## Make it yours
Open `index.html` and find the block near the top of the `<script>` marked:

    ✏️  EDIT YOUR DETAILS HERE

Edit these plain JS objects — the whole site updates from them:

- `PROFILE`    name, role, location, email, github, linkedin, resume URL
- `SKILLS`     grouped skills with 0–100 levels (rendered as ASCII bars)
- `PROJECTS`   name, tagline, description, stack, metrics, link
- `EXPERIENCE` roles with bullet points
- `EDUCATION`  degrees and certs

**ASCII name banner:** the big "ARJUN" art is the `BANNER_ART` constant.
Generate your own at patorjk.com/software/taag (font: "ANSI Shadow")
and paste the lines in.

**Fallback contact info:** also update the `<noscript>` block near the
top of the file (shown only when JavaScript is disabled).

## Commands visitors can run
help · about · skills · projects · experience · education · contact ·
resume · neofetch · nvidia-smi · train · theme · banner · clear
…plus ls, cat, echo, whoami, date, history, sudo hire-me, vim, rm -rf /
(try them).

Extras: ↑/↓ command history · Tab autocomplete · every command in the
output is clickable (works great on mobile).

## Themes
`theme night` (default) · `theme matrix` · `theme amber` · `theme paper`
— or click the ◐ button in the title bar to cycle.

## Deploy
It's one static file, so anything works:
- **GitHub Pages:** push to a repo → Settings → Pages → deploy from branch
- **Netlify / Vercel:** drag-and-drop the folder
- Any static host / S3 bucket / nginx

## Notes
- Font: JetBrains Mono via Google Fonts (graceful monospace fallback offline)
- Responsive down to phones; respects `prefers-reduced-motion`
- No frameworks, no tracking, no storage — view-source friendly
