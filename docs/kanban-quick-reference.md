# Kanban Quick Reference

## Board Columns
| Column | Purpose | Automation | WIP Limit |
|--------|---------|------------|-----------|
| **Backlog** | Future tasks | None | None |
| **To Do** | Ready to work | New/Reopened issues | None |
| **In Progress** | Being worked on | None | 3 per person |
| **In Review** | Awaiting review | New PRs | 5 total |
| **Done** | Completed | Closed issues/Merged PRs | None |

## Essential Labels
- **Priority**: `priority-high`, `priority-medium`, `priority-low`
- **Type**: `user-story`, `task`, `bug`, `enhancement`
- **Status**: `blocked`, `needs-info`, `ready-for-review`
- **Estimation**: `1-point`, `2-points`, `3-points`, `5-points`, `8-points`

## Story Points
- **1 point**: 1-2 hours (very simple)
- **2 points**: Half day (simple)
- **3 points**: 1 day (medium)
- **5 points**: 2-3 days (complex)
- **8 points**: 1 week (very complex)

## Quick Actions
- 🆕 **New Issue**: Use templates in Issues tab
- 🔀 **Move Card**: Drag and drop on project board
- 🏷️ **Add Labels**: Click label button on issue
- 👥 **Assign**: Use assignee dropdown
- 🔗 **Link PR**: Use "Closes #123" in PR description

## Daily Checklist
- [ ] Check board for updates
- [ ] Move started work to "In Progress"
- [ ] Update issue comments
- [ ] Move completed work to "In Review"
- [ ] Create PRs for finished code

## Branch Naming
- `feature/issue-123-description`
- `bugfix/issue-123-description`
- `hotfix/critical-issue`

## Commit Messages
```
Type: Brief description

- Closes #123
- Detailed explanation if needed
```

## Need Help?
- 📖 [Full Documentation](README.md#kanban-workflow)
- 🛠️ [Setup Guide](docs/kanban-setup-guide.md)
- 👥 [Team Workflow](docs/team-workflow.md)
- 📋 [Project Board](../../projects)