# Project Delivery Agent Templates

[中文版 / Chinese Version](./README.md)

This folder stores reusable templates for a project delivery team in Multica, covering roles such as product manager, project manager, frontend, backend, and QA.

## Contents

- `00-product-manager-prd.md`
  Full product manager role focused on requirement design and PRD generation

- `00-product-manager-instructions-short.md`
  Concise product manager instructions for the Multica agent `instructions` field

- `01-project-manager.md`
  Full project manager role definition

- `01-project-manager-instructions-short.md`
  Concise project manager instructions for the Multica agent `instructions` field

- `02-frontend-developer.md`
  Frontend developer role definition

- `03-backend-developer.md`
  Backend developer role definition

- `04-project-qa.md`
  Project QA role definition

- `05-routing-rules.md`
  Task routing rules for a coordinator or squad-style setup

- `07-sub-issue-splitting.md`
  Sub-issue splitting rules for the project manager

- `skills/product-manager-prd/SKILL.md`
  Importable PRD skill for the product manager

- `skills/project-manager-sub-issue-splitting/SKILL.md`
  Importable task-splitting skill for the project manager

## Usage

1. Copy the concise role definition into the agent `instructions` field in Multica.
2. Create a skill from the corresponding `SKILL.md` and attach it to the matching agent.
3. Use [05-routing-rules.md](/Users/madongyu/Documents/AgentCode/multica/docs/agent-role-templates/05-routing-rules.md) as the collaboration routing rules.
4. Adjust names, domain terminology, boundaries, and approval checkpoints to match your real project.

## Recommended Setup

- Product Manager:
  `instructions` -> `00-product-manager-instructions-short.md`
  `skill` -> `skills/product-manager-prd/SKILL.md`

- Project Manager:
  `instructions` -> `01-project-manager-instructions-short.md`
  `skill` -> `skills/project-manager-sub-issue-splitting/SKILL.md`

- Frontend Developer:
  `instructions` -> `02-frontend-developer.md`

- Backend Developer:
  `instructions` -> `03-backend-developer.md`

- Project QA:
  `instructions` -> `04-project-qa.md`

## Trigger Guidance

- If the work is still in the stage of ideas, goals, requirement clarification, PRD drafting, scope definition, or prioritization:
  use `skills/product-manager-prd/SKILL.md`

- If the requirement or PRD is already clear and now needs to be turned into parent issues, sub-issues, dependency order, and execution assignments:
  use `skills/project-manager-sub-issue-splitting/SKILL.md`

- If the work has already entered implementation, integration, or bug fixing:
  do not trigger the product manager or project manager skill; switch to the frontend or backend role

- If the work has already entered validation, regression, or release decision:
  do not trigger the product manager or project manager skill; switch to the QA role
