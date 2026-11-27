# NextID-Core

[English](README.md) · [Türkçe](README.tr.md) · [Core library](../README.md)

Shared open-source identity and access management foundation for NextID. The source comes directly from [keycloak/keycloak](https://github.com/keycloak/keycloak), not from the personal fork. The personal [muratdelen/NextID-Core](https://github.com/muratdelen/NextID-Core) is the architectural reference: its head `8ec0daff818713f106ebbd816581fbe6358f2557` adds only an upstream synchronization workflow to upstream commit `5274246ade2f0a4731ee5004cf29eec4ee58b4aa`. We pin the same original Keycloak source baseline, excluding the personal workflow.

- Upstream commit: [`5274246ade2f0a4731ee5004cf29eec4ee58b4aa`](https://github.com/keycloak/keycloak/commit/5274246ade2f0a4731ee5004cf29eec4ee58b4aa)
- Upstream tree: `5fc6d20afdd8a8f94210ad6a6715246b9dc3c010`
- License: Apache-2.0; preserve [original license](https://github.com/keycloak/keycloak/blob/5274246ade2f0a4731ee5004cf29eec4ee58b4aa/LICENSE.txt), copyright and notices.
- Source directory: `source/`, a Git submodule targeting the original upstream repository at that exact commit.

To materialize the full source code locally after checking out NextOpenSource:

```bash
git submodule update --init --recursive Core/NextID-Core/source
git -C Core/NextID-Core/source rev-parse HEAD
```

This retains the original Git history and repository structure without copying an entire independent fork into NextOpenSource's own history. GitHub stores the gitlink and pinned revision; code is fetched from Keycloak when the submodule is initialized. No HCC-specific source changes, product localization, credentials, or active synchronization workflow are introduced.

For future updates, fetch the upstream remote, select and review an explicit revision, assess security/licensing/build and regression evidence, then advance the gitlink through a reviewed PR. No automatic sync, build, deployment or production suitability is claimed. See [upstream record](UPSTREAM.md).
