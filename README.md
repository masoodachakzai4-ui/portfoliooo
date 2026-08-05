Jamie Chen — Developer Portfolio
A single-file, self-contained portfolio website for a software developer. No build step, no dependencies to install — just open `portfolio.html` in a browser or upload it to any host.
What's inside
`portfolio.html` contains everything: HTML, CSS, and your profile photo (embedded as base64), all in one file. There's nothing else to bundle or link.
Sections
Section	Purpose
Header / Profile card	Photo, name, role, availability status, quick contact line, and CTA buttons
About	Short bio — who you are, what you do, one concrete accomplishment
Experience & Projects	Chronological timeline of roles and projects, newest first
Skills	Toolkit grouped into Languages, Frontend, Backend, Infrastructure
Contact	Closing call-to-action with email, GitHub, and LinkedIn links
Design
Palette: navy (`#12293d`) as the primary accent, brass/gold (`#a9823c`) for highlights, on a warm off-white background
Type: Source Serif 4 for headings, Inter for body text, IBM Plex Mono for small labels/eyebrows
Layout: single column, responsive down to mobile, with a card-based profile header and a timeline for experience
How to customize
Everything is placeholder content. Open the file in any text editor and search for these to replace:
`Jamie Chen` — your name (appears in the nav, header, and page title)
`Full-Stack Software Developer` — your title
`[City, Country]`, `jamie.chen@example.com` — your location and contact info
The About paragraphs — swap in your real bio, previous company, and a measurable accomplishment
Each `.t-item` block in Experience & Projects — one block per role or project (title, company/context, description, tech tags)
The Skills pills — update to match your actual stack
The Contact section links — point `mailto:` and the GitHub/LinkedIn `href`s to your real profiles
The `Download résumé` button — currently `href="#"`; point it to a hosted PDF (e.g. `resume.pdf` if you upload one alongside this file)
Replacing the photo
The photo is embedded as a base64 data URI inside the single `<img class="profile-photo" src="data:image/jpeg;base64,...">` tag in the header. To swap it, replace that whole `src="..."` value with a data URI for your new image, or point it at an image URL/relative file path instead if you'd rather not embed it.
Publishing it
Since it's one static HTML file, you can host it for free on any of these:
GitHub Pages — push it to a repo, rename it `index.html`, enable Pages in repo settings
Netlify / Vercel — drag-and-drop the file onto their dashboard
Any static host — just upload `portfolio.html`
Notes
Fonts load from Google Fonts via CDN — an internet connection is needed for them to render (falls back to system fonts otherwise)
No JavaScript framework or build tools required
Tested responsive down to mobile widths; timeline collapses to a single column on small screens
