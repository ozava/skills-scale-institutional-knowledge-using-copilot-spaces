# Scale institutional knowledge using Copilot Spaces

This repository contains an interactive exercise for scaling institutional knowledge using GitHub Copilot Spaces.

Overview

OctoAcme uses Copilot Spaces to centralize, share, and maintain institutional knowledge. This docs/README provides a brief project overview and a summary of project management processes used by OctoAcme to manage content, reviews, and releases.

Goals

- Capture and centralize institutional knowledge in a living documentation site.
- Make updates discoverable and reviewable through GitHub workflows (issues, branches, and pull requests).
- Encourage cross-team collaboration through clear ownership and review processes.

How content is managed

1. Create an issue for new content or major changes describing the goal, scope, and desired outcome.
2. Create a feature branch named with the pattern `docs/<short-description>` or `feature/docs/<short-description>`.
3. Commit changes to the `docs/` folder and open a pull request that references the originating issue (e.g., "Closes #1").
4. Add reviewers and request a review via the PR interface. At least one content owner and one subject-matter expert must review documentation changes.
5. Once approvals are received and CI checks (if any) pass, merge the PR to the default branch.

OctoAcme project management processes (brief)

- Work tracking and planning:
  - OctoAcme uses an issue-driven workflow. New work starts with an issue describing the scope and acceptance criteria.
  - Issues are triaged and prioritized on a regular cadence (weekly triage meeting).
  - For longer-term efforts, Epics (or milestone grouping) are used to group related issues.

- Team collaboration and communication:
  - Teams use Copilot Spaces for shared context and to invite cross-functional contributors to participate in documentation and knowledge upkeep.
  - Regular syncs and asynchronous updates are documented in the Space and linked to relevant issues.

- Review and approval:
  - Documentation PRs must include at least one reviewer who is an owner of the content area and another who is a technical reviewer where applicable.
  - Use clear PR descriptions that link to the originating issue and list the reviewers requested (e.g., @ozava).

- Branching and merging:
  - Branch naming: `feature/<area>-<short-desc>` or `docs/<short-desc>`.
  - Squash or rebase merges are preferred for a linear history; include the issue number in the merged commit message.

- Release and maintenance:
  - Documentation changes are merged to the default branch and deployed according to release cadence (continuous or periodic releases).
  - Periodic audits (quarterly) review stale docs and update owners and labels.

Reviewer and PR guidance

- When opening a PR, reference the issue number and include a short summary of changes.
- Request specific reviewers (e.g., @ozava) in the PR so they receive a review request notification.
- Use labels such as `docs`, `review-needed`, and `good-first-issue` where appropriate.
