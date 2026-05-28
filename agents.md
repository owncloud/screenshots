# agents.md — screenshots

## Repository Overview

A central collection of screenshots for ownCloud software, organized by app and feature area. These images are used in documentation, marketing materials and presentations. The repository contains no code -- only image files organized in directories by ownCloud app name.

- **Classification:** Community / Meta
- **Activity Status:** Maintenance
- **License:** No license file detected (README states Creative Commons Attribution 4.0)
- **Language:** None (image assets only)

## Architecture & Key Paths

- `files/` — Screenshots of the Files app
- `sharing/` — Screenshots of sharing features
- `settings/` — Screenshots of admin/user settings
- `gallery/` — Screenshots of the Gallery app
- `calendar/` — Screenshots of the Calendar app
- `contacts/` — Screenshots of the Contacts app
- `Mobile/` — Mobile app screenshots
- `activity/` — Screenshots of the Activity app
- `oauth2/` — Screenshots of the OAuth2 app
- `README.md` — Contribution guidelines and screenshot standards

## Development Conventions

- Viewport resolution: 1280x720 pixels (widescreen)
- No browser chrome in screenshots (crop to ownCloud UI only)
- Use Gimp Pixelize filter (5x5) to obscure personal information
- Master branch holds latest stable release screenshots
- Older versions tracked in separate branches

## Build & Test Commands

No build or test commands. This is a static asset repository.

## Important Constraints

- **No license file detected:** The README states Creative Commons Attribution 4.0 but no formal LICENSE file exists. The OSPO is working on formalizing the license status as part of the Apache 2.0 migration.
- Do not introduce new **copyleft-licensed dependencies** (GPL, AGPL, LGPL, MPL) without explicit discussion in an issue first. This is especially important for repos that are migrating to or already under Apache 2.0, as copyleft dependencies would block or complicate that migration.
- **Content licensing:** Screenshot contributions must be CC-licensed or free content only.
- **No code:** This repository contains only image files.


## OSPO Policy Constraints

### GitHub Actions
- **Only** use actions owned by `owncloud`, created by GitHub (`actions/*`), verified on the GitHub Marketplace, or verified by the ownCloud Maintainers.
- Pin all actions to their full commit SHA (not tags): `uses: actions/checkout@<SHA> # vX.Y.Z`
- Never introduce actions from unverified third parties.

### Dependency Management
- Dependabot is configured for automated dependency updates.
- Review and merge Dependabot PRs as part of regular maintenance.
- Do not introduce new dependencies without discussion in an issue first.

### Git Workflow
- **Rebase policy**: Always rebase; never create merge commits. Use `git pull --rebase` and `git rebase` before pushing.
- **Signed commits**: All commits **must** be PGP/GPG signed (`git commit -S -s`).
- **DCO sign-off**: Every commit needs a `Signed-off-by` line (`git commit -s`).
- **Conventional Commits & Squash Merge**: Use the [Conventional Commits](https://www.conventionalcommits.org/) format where the repository enforces it. Many repos use squash merge, where the PR title becomes the commit message on the default branch — apply Conventional Commits format to PR titles as well. A reusable GitHub Actions workflow enforces this.

## Context for AI Agents

- This repository has no code, build system or CI.
- All content is organized by ownCloud app/feature name in subdirectories.
- Screenshots follow strict resolution and formatting guidelines documented in the README.
- The master branch represents the latest stable ownCloud release.
