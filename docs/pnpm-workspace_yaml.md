---
id: pnpm-workspace_yaml
title: pnpm-workspace.yaml
---

`pnpm-workspace.yaml` defines the root of the [workspace](workspaces) and it allows to
include/exclude directories from the workspace. By default, all packages
of all subdirectories are included.

An example of a `pnpm-workspace.yaml`:

```yaml
packages:
  # the root package.json
  - '.'
  # all packages in subdirs of packages/ and components/
  - 'packages/**'
  - 'components/**'
  # exclude packages that are inside test/ directories
  - '!**/test/**'
```
