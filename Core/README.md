# Core — shared open-source foundation

[English](README.md) · [Türkçe](README.tr.md) · [NextOpenSource](../README.md)

This directory is the shared catalog and source location for reusable open-source components acquired from third-party upstream projects for HCC. Each authorized component has its own stable directory under `Core/<ComponentID>/`.

```text
Core/
  README.md
  README.tr.md
  <ComponentID>/                 # one directory per upstream component
    README.md                    # origin, purpose, pinned version, use
    README.tr.md                 # equivalent Turkish documentation
    UPSTREAM.md                  # provenance and review record
    source/                      # authorized upstream source snapshot or Git submodule
    patches/                     # explicitly recorded HCC changes, if required
```

## Import and maintenance rules

- Before importing, record the upstream repository URL, exact commit/tag, license and required notices, maintenance status, dependencies, security review, intended HCC use and human approval. Use [the upstream record template](../templates/UPSTREAM.md).
- Preserve original license/notice files, attribution and upstream provenance with source. Prefer a verified, pinned upstream revision; use a separately maintained Core repository or a submodule reference where appropriate instead of duplicating an existing Core repository. Keep original source and HCC-specific changes traceable.
- Do not mix product-specific localized data, confidential information, presentation assets or proprietary source into the upstream baseline. Keep product adaptations in the relevant independent product repository; keep unavoidable Core patches separately documented and reviewed.
- Validate updates, license compatibility and security through the applicable review process; link test evidence from NextSecurity. Do not import code whose licensing or provenance is unresolved, and do not assume a license merely because a repository is private.
- Project-specific evaluation and integration plans belong in the relevant project directory in NextOpenSource and NextRoadmap; reuse this common component library rather than copying it into each project.

## Registered components

| Component | Upstream | Pinned revision | License | State |
|---|---|---|---|---|
| [NextID-Core](NextID-Core/README.md) | [Keycloak](https://github.com/keycloak/keycloak) | [`5274246ade2f`](https://github.com/keycloak/keycloak/commit/5274246ade2f0a4731ee5004cf29eec4ee58b4aa) | Apache-2.0 | Git submodule; source available on recursive checkout; security/build verification pending |

Add further components after relevant review and authorization.
