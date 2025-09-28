# Kanban Board Setup Guide

This guide will help you set up and configure the GitHub Project board for this repository.

## Step 1: Create a New Project

1. Navigate to the repository's **Projects** tab
2. Click **"New project"**
3. Choose **"Board"** layout
4. Name it **"Kanban Board"**
5. Add description: **"Main project board for tracking all work using Kanban methodology"**

## Step 2: Configure Columns

Create the following columns in order:

### Backlog
- **Purpose**: Ideas and future tasks that haven't been prioritized yet
- **Automation**: None
- **WIP Limit**: None

### To Do
- **Purpose**: Prioritized tasks ready to be worked on  
- **Automation**: 
  - ✅ Newly added issues
  - ✅ Reopened issues
- **WIP Limit**: None

### In Progress
- **Purpose**: Tasks currently being worked on
- **Automation**: None
- **WIP Limit**: 3 per assignee

### In Review
- **Purpose**: Tasks completed and awaiting review/testing
- **Automation**: 
  - ✅ Newly added pull requests
- **WIP Limit**: 5 total

### Done
- **Purpose**: Completed and verified tasks
- **Automation**: 
  - ✅ Closed issues
  - ✅ Merged pull requests
- **WIP Limit**: None

## Step 3: Set Up Labels

Create these labels in the repository (**Issues** → **Labels** → **New label**):

### Priority Labels
- `priority-high` (Color: #d73a4a)
- `priority-medium` (Color: #fbca04)  
- `priority-low` (Color: #0075ca)

### Type Labels
- `user-story` (Color: #7057ff)
- `task` (Color: #a2eeef)
- `bug` (Color: #d73a4a)
- `enhancement` (Color: #84b6eb)

### Status Labels
- `blocked` (Color: #b60205)
- `needs-info` (Color: #d4c5f9)
- `ready-for-review` (Color: #0e8a16)

### Estimation Labels  
- `1-point` (Color: #c2e0c6)
- `2-points` (Color: #bfd4f2)
- `3-points` (Color: #f9d0c4)
- `5-points` (Color: #fef2c0)
- `8-points` (Color: #f7c6c7)

## Step 4: Enable Automation

The repository includes a GitHub Actions workflow (`.github/workflows/kanban-automation.yml`) that automatically:

- Moves new issues to "To Do"
- Moves reopened issues to "To Do"  
- Moves closed issues to "Done"
- Moves new pull requests to "In Review"
- Moves merged pull requests to "Done"

## Step 5: Create Sample Issues

Use the issue templates to create sample issues:

1. **Sample User Story**: Create a login feature
2. **Sample Task**: Set up development environment
3. **Sample Bug**: Fix navigation menu on mobile

## Step 6: Test the Workflow

1. Create a new issue using one of the templates
2. Verify it appears in "To Do" column
3. Move it to "In Progress" when starting work
4. Create a pull request and verify it appears in "In Review"
5. Merge the pull request and verify it moves to "Done"

## Best Practices

- Review and update the board daily
- Respect WIP limits to maintain flow
- Use consistent labeling for better tracking
- Link pull requests to issues for better traceability
- Regularly groom the backlog during team meetings

## Troubleshooting

### Issues not moving automatically
- Check that the GitHub Actions workflow is enabled
- Verify that the project name matches exactly ("Kanban Board")
- Ensure column names match the workflow configuration

### Labels not appearing
- Make sure labels are created at the repository level
- Check that issue templates reference the correct label names

### Automation not working
- Verify that the repository has Actions enabled
- Check the Actions tab for any failed workflow runs
- Ensure the workflow has proper permissions