# 项目交付智能体模板

[English Version](./README.en.md)

这个目录存放一套适用于 Multica 的项目交付团队模板，主要用于配置产品经理、项目经理、前后端开发、验收等角色。

## 文件清单

- `00-product-manager-prd.md`
  产品经理完整角色说明，聚焦需求设计与 PRD 产出

- `00-product-manager-instructions-short.md`
  适合直接粘贴到 Multica agent `instructions` 的产品经理短版设定

- `01-project-manager.md`
  项目经理完整角色说明

- `01-project-manager-instructions-short.md`
  适合直接粘贴到 Multica agent `instructions` 的项目经理短版设定

- `02-frontend-developer.md`
  前端开发角色说明

- `03-backend-developer.md`
  后端开发角色说明

- `04-project-qa.md`
  项目验收角色说明

- `05-routing-rules.md`
  任务路由规则，适合放在协作协调者或 squad 说明中

- `07-sub-issue-splitting.md`
  项目经理的子 issue 拆分规则

- `skills/product-manager-prd/SKILL.md`
  可导入的产品经理 PRD skill

- `skills/project-manager-sub-issue-splitting/SKILL.md`
  可导入的项目经理子任务拆分 skill

## 使用方式

1. 将对应角色的短版设定复制到 Multica 的 agent `instructions` 字段。
2. 将对应的 `SKILL.md` 内容创建为 skill，并挂载到对应 agent。
3. 将 [05-routing-rules.md](/Users/madongyu/Documents/AgentCode/multica/docs/agent-role-templates/05-routing-rules.md) 用作协作路由规则。
4. 根据你的真实项目调整名称、领域术语、边界和确认点。

## 推荐搭配

- 产品经理：
  `instructions` -> `00-product-manager-instructions-short.md`
  `skill` -> `skills/product-manager-prd/SKILL.md`

- 项目经理：
  `instructions` -> `01-project-manager-instructions-short.md`
  `skill` -> `skills/project-manager-sub-issue-splitting/SKILL.md`

- 前端开发师：
  `instructions` -> `02-frontend-developer.md`

- 后端开发师：
  `instructions` -> `03-backend-developer.md`

- 项目验收师：
  `instructions` -> `04-project-qa.md`
