# Lloyds_DA_AI_Scientist_Take_Home

## Project Management with Kanban

This repository uses a Kanban methodology for project management to ensure efficient workflow and transparent progress tracking.

### Kanban Board Structure

Our Kanban board consists of the following columns:

1. **Backlog** - Ideas and future tasks that haven't been prioritized yet
2. **To Do** - Prioritized tasks ready to be worked on
3. **In Progress** - Tasks currently being worked on
4. **In Review** - Tasks completed and awaiting review/testing
5. **Done** - Completed and verified tasks

### Getting Started with the Kanban Board

#### Accessing the Board
- Navigate to the [Projects tab](https://github.com/drOluOla/Lloyds_DA_AI_Scientist_Take_Home/projects) in this repository
- Select "Kanban Board" to view the current project status

#### Creating Issues
Use our predefined issue templates to maintain consistency:

- **User Stories** - For feature requests and user-focused requirements
- **Tasks** - For development tasks and technical work
- **Bug Reports** - For reporting and tracking bugs

#### Workflow Process

1. **Planning Phase**
   - Create issues using appropriate templates
   - Add labels for categorization (`user-story`, `task`, `bug`, `priority-high`, etc.)
   - Assign story points or time estimates
   - Place new items in the "Backlog" column

2. **Development Phase**
   - Move items from "Backlog" to "To Do" during sprint planning
   - Assign items to team members
   - Move to "In Progress" when work begins
   - Create pull requests linked to issues

3. **Review Phase**
   - Move completed work to "In Review"
   - Conduct code reviews
   - Perform testing and quality assurance

4. **Completion Phase**
   - Move verified items to "Done"
   - Close related issues and pull requests

### Kanban Best Practices

#### Work in Progress (WIP) Limits
- **In Progress**: Maximum 3 items per person
- **In Review**: Maximum 5 items total

#### Definition of Done
- [ ] Code is written and tested
- [ ] Code review completed
- [ ] Documentation updated
- [ ] All acceptance criteria met
- [ ] No critical bugs identified

#### Labels and Prioritization
- **Priority**: `priority-high`, `priority-medium`, `priority-low`
- **Type**: `user-story`, `task`, `bug`, `enhancement`
- **Status**: `blocked`, `needs-info`, `ready-for-review`
- **Estimation**: `1-point`, `2-points`, `3-points`, `5-points`, `8-points`

### Automation Features

The repository includes automated workflows that:
- Automatically move new issues to "To Do"
- Move reopened issues back to "To Do"
- Move closed issues to "Done"
- Move new pull requests to "In Review"
- Move merged pull requests to "Done"

### Team Collaboration

#### Daily Standups
Use the Kanban board to facilitate daily standups:
- What did you complete yesterday?
- What are you working on today?
- Are there any blockers?

#### Sprint Planning
- Review and prioritize items in the "Backlog"
- Move selected items to "To Do"
- Ensure WIP limits are respected
- Assign items to team members

#### Retrospectives
- Analyze flow metrics (cycle time, lead time)
- Identify bottlenecks in the process
- Continuously improve the workflow

### Getting Help

- Check the [issue templates](.github/ISSUE_TEMPLATE/) for guidance on creating well-structured issues
- Review the [kanban automation workflow](.github/workflows/kanban-automation.yml) to understand automated processes
- Refer to this documentation for workflow questions