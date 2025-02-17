---
title: "About global configs"
id: "about-global-configs"
sidebar: "About global configs"
---

Global configs enable you to fine-tune _how_ dbt runs projects on your machine—whether your personal laptop, an orchestration tool running remotely, or (in some cases) dbt Cloud. In general, they differ from most [project configs](/reference/dbt_project.yml) and [resource configs](/reference/configs-and-properties), which tell dbt _what_ to run.

Global configs control things like the visual output of logs, the manner in which dbt parses your project, and what to do when dbt finds a version mismatch or a failing model. These configs are "global" because they are available for all dbt commands, and because they can be set for all projects running on the same machine or in the same environment.

Starting in v1.0, you can set global configs in three places. When all three are set, command line flags take precedence, then environment variables, and last yaml configs (usually `profiles.yml`).