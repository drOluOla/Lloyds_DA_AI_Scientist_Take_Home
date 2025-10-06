# Team Workflow with Kanban

This document outlines how the team should use the Kanban board for effective collaboration.

## Daily Workflow

### Starting Your Day
1. Check the Kanban board for updates
2. Review items assigned to you in "To Do" 
3. Move any item you're starting to "In Progress"
4. Update issue comments with your plan for the day

### During Development
1. Keep issue comments updated with progress
2. Ask questions in issue comments if blocked
3. Add the `blocked` label if you can't proceed
4. Link related pull requests to issues

### End of Day
1. Update issue comments with progress made
2. Move completed work to "In Review"
3. Ensure pull requests are created and linked

## Weekly Rituals

### Monday: Sprint Planning
1. Review and prioritize "Backlog" items
2. Move selected items to "To Do"
3. Assign items to team members
4. Estimate effort using story points
5. Set sprint goals

### Wednesday: Mid-Sprint Check
1. Review board for bottlenecks
2. Help unblock any "blocked" items
3. Adjust assignments if needed
4. Update estimates if required

### Friday: Sprint Review & Retrospective
1. Review completed work in "Done"
2. Demo finished features
3. Discuss what went well
4. Identify areas for improvement
5. Plan improvements for next sprint

## Issue Management

### Creating Quality Issues

#### User Stories
```markdown
As a [user type], I want [functionality] so that [benefit].

Acceptance Criteria:
- [ ] Specific, testable criterion 1
- [ ] Specific, testable criterion 2
- [ ] Specific, testable criterion 3
```

#### Tasks
```markdown
Task: [Clear, actionable description]

Objectives:
- [ ] Objective 1
- [ ] Objective 2
- [ ] Objective 3

Dependencies: [List any blockers]
```

#### Bug Reports
```markdown
Bug: [Brief description]

Steps to Reproduce:
1. Step 1
2. Step 2
3. Step 3

Expected: [What should happen]
Actual: [What actually happens]
```

### Labeling Strategy

#### Required Labels
- **Type**: `user-story`, `task`, `bug`, `enhancement`
- **Priority**: `priority-high`, `priority-medium`, `priority-low`

#### Optional Labels
- **Estimation**: `1-point`, `2-points`, `3-points`, `5-points`, `8-points`
- **Status**: `blocked`, `needs-info`, `ready-for-review`

### Story Point Guidelines

| Points | Complexity | Time Estimate |
|--------|------------|---------------|
| 1      | Very Simple | 1-2 hours |
| 2      | Simple | Half day |
| 3      | Medium | 1 day |
| 5      | Complex | 2-3 days |
| 8      | Very Complex | 1 week |

## Pull Request Process

### Creating Pull Requests
1. Create a feature branch from main
2. Make focused, atomic commits
3. Write clear commit messages
4. Link to related issues using "Closes #123"
5. Request appropriate reviewers

### Review Process
1. Reviewer checks out the branch locally
2. Tests the changes thoroughly
3. Reviews code for quality and standards
4. Approves or requests changes
5. Merges when approved

### Branch Naming Convention
- Feature: `feature/issue-123-short-description`
- Bug Fix: `bugfix/issue-123-short-description`
- Hotfix: `hotfix/critical-issue-description`

## Team Roles & Responsibilities

### Product Owner
- Prioritizes backlog items
- Writes and refines user stories
- Accepts completed work
- Makes scope decisions

### Scrum Master/Facilitator
- Facilitates team meetings
- Removes blockers
- Monitors team metrics
- Coaches team on process

### Developers
- Estimate work effort
- Complete assigned tasks
- Review others' code
- Maintain code quality

### QA/Testers
- Test completed features
- Report bugs
- Verify acceptance criteria
- Maintain test documentation

## Metrics & Improvement

### Key Metrics to Track
- **Cycle Time**: Time from "In Progress" to "Done"
- **Lead Time**: Time from "To Do" to "Done"
- **Throughput**: Items completed per sprint
- **WIP**: Number of items in progress
- **Blocked Time**: Time items spend blocked

### Monthly Review Questions
1. Are we meeting our sprint commitments?
2. Where are the bottlenecks in our process?
3. Are our estimates accurate?
4. How can we improve our cycle time?
5. What blockers can we prevent?

## Communication Guidelines

### Issue Comments
- Use @mentions to notify specific people
- Be specific and actionable
- Include context and links
- Update progress regularly

### Stand-up Format
- What did I complete yesterday?
- What will I work on today?
- What is blocking me?
- How can I help others?

### Retrospective Format
- **Start**: What should we start doing?
- **Stop**: What should we stop doing?  
- **Continue**: What should we keep doing?
- **Action Items**: Specific improvements to implement

## Tools Integration

### GitHub Integration
- Link pull requests to issues
- Use project automation rules
- Leverage GitHub Actions
- Use draft pull requests for work-in-progress

### External Tools
- Slack/Teams for daily communication
- Video calls for complex discussions
- Shared documents for specifications
- Time tracking tools if required

## Troubleshooting Common Issues

### Items stuck in "In Progress"
- Check if developer needs help
- Review if scope is too large
- Consider breaking into smaller tasks
- Remove blockers quickly

### Too many items in "In Review"
- Add more reviewers
- Simplify review process
- Improve code quality practices
- Set review time expectations

### Backlog growing too large
- Regular backlog grooming
- Archive outdated items
- Prioritize ruthlessly
- Focus on MVP features