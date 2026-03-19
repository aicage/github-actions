# GitHub Actions (shared)

> [!WARNING]
> **This repository is archived and should not be adopted for new work.**
> Migrate multi-arch publish/sign/provenance usage to
> [`gh-workflow/multiarch-image-build-sign-provenance`](https://github.com/gh-workflow/multiarch-image-build-sign-provenance).

Shared workflows and custom composite actions for aicage repositories.

## Included

- Reusable workflow: multi-arch build, sign, and provenance publishing
- Composite action: multi-arch publish, sign, and provenance validation
- Helper composite actions used by the workflow and the top-level composite action

## Usage

Consume the workflow via `workflow_call` and pass `actions_ref` to pin the actions to the same git ref.

Use `.github/actions/multiarch-image-build-sign-provenance` when the signing identity must stay with the caller
workflow. The caller job must provide the required permissions, in particular `packages: write` and `id-token: write`.
