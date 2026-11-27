# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md)

Shared open-source identity and access management foundation for NextID. Original source from [keycloak/keycloak](https://github.com/keycloak/keycloak); the personal fork is a structural reference, not the source. No original upstream file has been intentionally changed.

- Upstream release: [26.8.2](https://github.com/keycloak/keycloak/releases/tag/26.8.2) (2026-11-05).
- Pinned commit: [`e514445f9dcdabc5bdcf67cab56c1e49655de067`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067)
- Source tree: `6f439a9bda71c39bf725150cea5d50f149e423f6`
- License: Apache-2.0; original license, attribution and notices are in the source.
- Source: [source/](source/), the full exact upstream Git tree as ordinary files.

A normal clone of NextOpenSource contains the complete source tree; no submodule initialization is needed. NextID can use the pinned source as build input. Its own independent repository holds localized data, themes, extensions, Dockerfile and product configuration.

The existing personal NextID is based on a Core container image and adds a NextLog listener extension. The future HCC delivery model separates original Keycloak source, reviewed Core build artifact and customized NextID product image. Neither a build nor image publication is authorized by this source registration. For build reproducibility, record the exact NextOpenSource commit and resulting image digest; avoid relying on floating `latest`. This repository is public; do not place credentials in Dockerfiles.

Update the upstream snapshot only through a reviewed PR, verify exact expected tree, retain upstream license and notices, and perform NextSecurity assessment, build and regression tests before production use. No automatic update or publication is enabled.
