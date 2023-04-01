---
description: >-
  This page contains all code conventions which are specific to the Mobile
  Application project, we expect these to be upheld in any contribution, and we
  enforce these.
---

# Project Conventions

## Naming Conventions <a href="#naming-conventions" id="naming-conventions"></a>

### Camel case for variables

```
❌ final StartAt = DateTime.now();
❌ final startat = DateTime.now();
✅ let startAt = DateTime.now();
```

### Snake Case File naming

```
❌ forumpermission.dart
❌ forum-permission.dart
✅ forum_permission.dart
```

### Pascal Case for Classes and Interfaces

```
❌ class userBloc {}
❌ class USER_BLOC {}
✅ class UserBloc {}
```

### Suffix DTOs with **Dto**

```
❌ class CrowdActionModel {}
✅ class CrowdActionDto {}
```

### Camel Case for Enum Properties and Constants

```
❌ const POINTS_PER_COMMITMENT = 50;
✅ const pointsPerCommitment = 50;

✅  enum CrowdActionType {
✅    food,
✅    energy,
✅  }

❌  enum CrowdActionType {
❌    FOOD,
❌    ENERGY,
❌  }
```
