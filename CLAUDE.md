# Project Context

This is a personal academic website built on the **AcademicPages** template
(a fork of Minimal Mistakes for Jekyll), hosted on GitHub Pages.

Owner: ECE student at UIUC. Content focus: embedded systems, hardware,
robotics coursework, and personal projects.

## Structure

- `_config.yml` — site-wide settings, author bio, social links
- `_pages/` — static pages (about, cv, publications index)
- `_portfolio/` — one `.md` per project, with YAML front matter
- `_publications/`, `_talks/` — same pattern, one file per entry
- `_data/navigation.yml` — top nav bar
- `_sass/`, `assets/css/main.scss` — style overrides
- `files/` — PDFs and downloadable assets
- `images/` — image assets

## Rules

1. **Never edit theme internals.** Minimal Mistakes is a remote/gem theme.
   All style changes go in `_sass/` or `assets/css/main.scss` as overrides.
   Do not modify anything under the theme gem directory.
2. **Match existing conventions.** Before creating a new collection entry,
   read an existing file in that folder and mirror its front-matter fields
   and formatting exactly.
3. **Front matter is not optional.** Every collection item needs at minimum
   `title`, `collection`, `permalink`. Malformed YAML breaks the build
   silently on GitHub Pages.
4. **Test before declaring done.** Run `bundle exec jekyll serve` and confirm
   the build succeeds with no warnings. Report any Liquid or YAML errors.
5. **Do not invent content.** Do not fabricate publications, dates, metrics,
   affiliations, or project details. If information is missing, leave a
   `TODO:` marker and ask.
6. **Small, reviewable changes.** Prefer several focused edits over one large
   rewrite. Explain what changed and why before I commit.
7. **Don't commit or push.** Leave that to me.

## Commands

- Local preview: `bundle exec jekyll serve`
- Install deps: `bundle install`

## Style

- Prose: plain, concise, first person. No marketing tone.
- Technical writing: specific over vague — name the chip, the protocol, the tool.
- Keep the existing color scheme unless I explicitly ask to change it.
