# GitHub Actions (shared)

Shared workflows and custom composite actions for aicage repositories.

## Included

- Reusable workflow: multi-arch build, sign, and provenance publishing
- Composite actions used by the workflow

## Usage

Consume the workflow via `workflow_call` and pass `actions_ref` to pin the actions to the same git ref.
