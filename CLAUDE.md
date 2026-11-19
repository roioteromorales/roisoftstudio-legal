# RoiSoftStudio Legal — Claude Code Instructions

Shared legal pages (privacy policies) for every published RoiSoftStudio game, served by **GitHub Pages**.

| | |
|---|---|
| Repo | https://github.com/roioteromorales/roisoftstudio-legal |
| Site | https://roioteromorales.github.io/roisoftstudio-legal/ |
| Stack | Jekyll (`_config.yml`, theme `minima`), plain Markdown pages |
| Deploy | **Every push to `main` rebuilds and publishes the site** (`pages-build-deployment`, GitHub-managed) |

## Structure

```
index.md                        landing page: one link per policy
{game-name}.md                  one privacy policy per game, served at /{game-name}
_config.yml                     Jekyll config
```

## Adding a privacy policy for a new game

Follow the template and steps in [games/CLAUDE.md — Privacy Policy](../CLAUDE.md#privacy-policy) (single source).
Two things that are easy to forget:

- Add the link to `index.md` too — the page works without it, but the landing page then does not list it.
- The URL the Play Console asks for is `https://roioteromorales.github.io/roisoftstudio-legal/{game-name}`;
  check it loads after the push (Pages takes a minute or two).

## Rules

- Everything here is public: no personal data, no addresses, only "RoiSoftStudio" as the developer name.
- A policy states what the game really does with data. When a game adds analytics, ads or a leaderboard
  (Play Games Services), update its policy and its "Last updated" date in the same change.
- Workspace conventions: [git workflow](../../docs/git-workflow.md), roadmap in [docs/roadmap.md](docs/roadmap.md).
