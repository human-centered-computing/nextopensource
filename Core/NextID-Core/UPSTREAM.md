# NextID-Core — upstream source record

- Source: https://github.com/keycloak/keycloak
- Pinned commit: 5274246ade2f0a4731ee5004cf29eec4ee58b4aa
- Source tree: 5fc6d20afdd8a8f94210ad6a6715246b9dc3c010
- Acquired: 2026-11-27 (Git submodule pointer; no standalone source archive stored)
- Personal model: muratdelen/NextID-Core, fork head 8ec0daff818713f106ebbd816581fbe6358f2557 — inspected diff adds only .github/workflows/sync-upstream.yml; that workflow is not imported.
- Parent/upstream relation verified against the actual Keycloak repository; selected commit is in the ancestry of upstream main at inspection time.
- License: Apache-2.0, original LICENSE.txt and per-file attribution retained in unmodified upstream source.
- Purpose: reusable Keycloak core identity and access management baseline for NextID; product source and localizations remain separate.
- Import strategy: pinned Git submodule at Core/NextID-Core/source (original upstream URL), preserving entire upstream tree and history on checkout.
- Maintenance: future version changes must go through reviewed PRs; no automatic schedule or new workflow activated. The selected historical baseline is not asserted to be the latest release.
- Security/build/functional acceptance: not performed in this change. NextSecurity review and exact-revision tests required before production use.
- Authorization: human maintainer requested adapting the original upstream fork pattern directly under NextOpenSource/Core. Review and approval of this source registration, and separate approval for implementation/release, remain required.
