---
description: >-
  This page contains all code conventions which are specific to the Backend
  project, we expect these to be upheld in any contribution, and we enforce
  these.
---

# Project Conventions

## Naming Conventions <a href="#naming-conventions" id="naming-conventions"></a>

### Camel case for variables

```
❌ let StartAt = new Date();
❌ let startat = new Date();
✅ let startAt = new Date();
```

### File naming

```
❌ forumpermission.entity.ts
✅ forum-permission.entity.ts
```

### Pascal Case for Classes and Interfaces

```
❌ class userService {}
❌ class USER_SERVICE {}
✅ class UserService {}
```

### Prefix Interfaces with **I**

```
❌ Interface iCrowdAction {}
❌ Interface CrowdActionInterface {}
✅ Interface ICrowdAction {}
```

### Suffix Enums with **Enum**

```
❌ enum CrowdActionStatus {}
✅ enum CrowdActionStatusEnum {}
```

### Suffix DTOs with **Dto**

```
❌ class CrowdActionModel {}
✅ class CrowdActionDto {}
```

### Screaming Snake Case for Enum Properties and Constants

```
❌ const pointsPerCommit: number = 50;
✅ const POINTS_PER_COMMIT: number = 50;
```
