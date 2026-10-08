# Seerr Fork Memory

## Reason for Fork
This fork contains security improvements to address missing permission checks on various administrative endpoints. The changes were made to ensure that only users with administrative privileges can perform sensitive operations such as regenerating API keys, modifying network settings, controlling scheduled jobs, and managing integrations.

## Changes Made
- Added `isAuthenticated(Permission.ADMIN)` middleware to the following endpoints in `/appdata/seerr/server/routes/settings/index.ts`:
  - `POST /main/regenerate`
  - `GET /network`
  - `POST /network`
  - `GET /jobs`
  - `POST /jobs/:jobId/run`
  - `POST /jobs/:jobId/cancel`
  - `POST /jobs/:jobId/schedule`
  - `GET /plex`
  - `POST /plex`
  - `GET /plex/library`
  - `PUT /plex/library/:libraryId`
  - `POST /plex/library/sync`
  - `GET /plex/sync`
  - `POST /plex/sync`
  - `GET /plex/users`
  - `GET /jellyfin`
  - `POST /jellyfin`
  - `GET /jellyfin/library`
  - `PUT /jellyfin/library/:libraryId`
  - `POST /jellyfin/library/sync`
  - `GET /jellyfin/users`
  - `GET /jellyfin/sync`
  - `POST /jellyfin/sync`
  - `GET /tautulli`
  - `POST /tautulli`
  - `GET /cache`
  - `POST /cache/:cacheId/flush`
  - `POST /cache/dns/:dnsEntry/flush`
  - `GET /main`
  - `POST /main`

## Relationship to Upstream
This fork is based on the upstream Seerr repository (https://github.com/seerr-team/seerr) at the `develop` branch. The changes are intended to be submitted as a pull request to the upstream repository.

## Local Development Notes
- The code-review-graph was updated after making these changes to reflect the new code structure.
- Remember to fork you support: if you use this fork, you are responsible for maintaining it and keeping it up to date with upstream if desired.