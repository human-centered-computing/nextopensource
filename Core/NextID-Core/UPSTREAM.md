# NextID-Core — upstream source record

- Source: https://github.com/keycloak/keycloak
- Release: 26.8.2, latest stable upstream release at review on 2026-11-27; published 2026-11-05. Verified via GitHub latest-release endpoint; not a draft or prerelease.
- Release URL: https://github.com/keycloak/keycloak/releases/tag/26.8.2
- Pinned commit: e514445f9dcdabc5bdcf67cab56c1e49655de067
- Source tree: 6f439a9bda71c39bf725150cea5d50f149e423f6
- Acquired: 2026-11-27 (Git submodule pointer; no standalone source archive stored).
- Personal model: muratdelen/NextID-Core is an upstream Keycloak fork with an added sync workflow. Used as a structural reference only; no personal fork code or workflow imported. Human maintainer explicitly requested the latest upstream release, rather than the personal fork baseline.
- License: Apache-2.0, original LICENSE.txt and per-file attribution retained in unmodified upstream source.
- Purpose: reusable Keycloak core identity and access management baseline for NextID; product source and localizations remain separate.
- Import strategy: pinned Git submodule at Core/NextID-Core/source (original upstream URL), preserving the exact release tree and history on checkout.
- Maintenance: future version changes must go through reviewed PRs; no automatic schedule or new workflow activated.
- Security/build/functional acceptance: not performed in this change. NextSecurity review and exact-revision tests required before production use.
- Authorization: human maintainer requested original upstream fork pattern directly under NextOpenSource/Core, using the latest release. Review and approval of this source registration, and separate approval for implementation/release, remain required.
