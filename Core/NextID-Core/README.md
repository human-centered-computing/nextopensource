# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Core library](../README.md)

Shared open-source identity and access management foundation for NextID. The source comes directly from [keycloak/keycloak](https://github.com/keycloak/keycloak), not from the personal fork. The personal [muratdelen/NextID-Core](https://github.com/muratdelen/NextID-Core) is the architectural reference only. At the maintainer's direction, this workspace uses the latest stable upstream release rather than the older personal fork baseline or its synchronization workflow.

- Latest stable upstream release at review: [26.8.2](https://github.com/keycloak/keycloak/releases/tag/26.8.2) (2026-11-05).
- Upstream commit: [`e514445f9dcdabc5bdcf67cab56c1e49655de067`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067)
- Upstream tree: `6f439a9bda71c39bf725150cea5d50f149e423f6`
- License: Apache-2.0; preserve [original license](https://github.com/keycloak/keycloak/blob/e514445f9dcdabc5bdcf67cab56c1e49655de067/LICENSE.txt), copyright and notices.
- Source directory: `source/`, a Git submodule targeting the original upstream repository at that exact commit.

To materialize the full source code locally after checking out NextOpenSource:

```bash
git submodule update --init --recursive Core/NextID-Core/source
git -C Core/NextID-Core/source rev-parse HEAD
```

This retains the original Git history and repository structure without copying an entire independent fork into NextOpenSource's own history. GitHub stores the gitlink and pinned revision; code is fetched from Keycloak when the submodule is initialized. No HCC-specific source changes, product localization, credentials, or active synchronization workflow are introduced.

For future updates, fetch the upstream remote, select and review an explicit revision, assess security/licensing/build and regression evidence, then advance the gitlink through a reviewed PR. No automatic sync, build, deployment or production suitability is claimed. See [upstream record](UPSTREAM.md).
