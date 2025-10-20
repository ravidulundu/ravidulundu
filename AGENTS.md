# Repository Guidelines

This repository powers the `ravidulundu` profile README. Keep additions
purposeful and easy for visitors to scan. Always preview Markdown updates in a
GitHub-flavored renderer before opening a pull request.

## Project Structure & Module Organization

- `README.md`: canonical profile content; changes here update the GitHub
  profile page.
- `github-header-image.png`: header artwork shown at the top of the README.
- Use an `assets/` directory for new media and reference files with relative
  paths such as `./assets/...`. Keep assets under 500 KB.

## Build, Test, and Development Commands

- `npx markdownlint-cli@latest README.md AGENTS.md`: lint Markdown for common
  style regressions.
- `npx remark-cli README.md --use remark-validate-links`: optionally check
  internal and external links.
- `npx prettier@latest --check README.md AGENTS.md`: verify formatting when you
  rely on Prettier for wrapping lists or tables.

## Coding Style & Naming Conventions

- Prefer GitHub Markdown. Maintain a shallow heading hierarchy without skipping
  levels.
- Write headings in sentence case and keep emoji usage consistent with existing
  sections.
- Limit tables to three columns and concise cell content for responsiveness.
- Name files in lowercase with hyphens, for example `github-header-image.png`.

## Testing Guidelines

- Run Markdown linting and link validation before submitting a pull request.
  Share command output if warnings remain.
- When changing media, confirm the README renders well in both GitHub themes.
- Ensure badges and external embeds resolve via HTTPS and fail gracefully.

## Commit & Pull Request Guidelines

- Follow Conventional Commits (for example `fix: align tech stack badges...`).
- Squash related edits into a single logical commit with subjects under 72
  characters.
- Provide concise summaries, screenshots for visual updates, and links to
  related issues.
- Enable "Allow edits" so maintainers can handle minor touch-ups without
  delaying reviews.
