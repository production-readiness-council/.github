# Branch Protection Baseline

This document records the default branch protection policy the organization should apply to public governance and workflow repositories.

## Repositories in scope

At minimum, apply these rules to:

- `.github`
- `governance`
- `proposals`

## Baseline rules

- protect the default branch
- require pull requests before merging
- require at least one approving review
- dismiss stale approvals when new commits are pushed
- require conversation resolution before merge
- block force pushes
- block branch deletion by non-admin contributors
- require status checks once CI or policy checks exist

## Administrative expectations

- direct pushes to the default branch should be avoided except for urgent repository bootstrapping by an owner or maintainer
- governance changes should merge only through pull requests with visible rationale
- publication or governance authority should not be inferred from admin bypass capability

## Future tightening

When maintainer and council teams exist, extend the baseline with:

- CODEOWNERS-enforced review requirements
- team-based review ownership
- separate protection rules for governance-critical paths
- repository rulesets for tag and branch naming constraints
