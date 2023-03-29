---
description: >-
  Our branching conventions describes how to name branches, and what information
  we expect your branch to contain.
---

# Branching Conventions

We use simple naming conventions for branches, to easily navigate and track multiple branches across features. Branches follow a 3 part logic, the first part describes the type of work is being done on the branch.

Often used tags are: `feat`, `feature`, `chore`, `task`, `refac`, `refactor`, `fix`, `bugfix`, `docs`, `documentation`, etc.

The second part is what issue or feature the branch relates to. This is used by taking the issue number, and prefixing it with `gh-`.

Examples: `gh-97`, `gh-104`, etc.

The third and last part describes the scope, it's okay to be generic if the scope is not easily defined. Multiple branches can have a similar name, and thus the scope helps differentiate and specify what exactly the branch pertains to. All words in the scope must be separated by `-`.

Examples: `profile-avatar`, `profile-settings`, `auth-new-user`, `crowdaction-details`, etc.

These three parts are separated by a slash (`/`), and concatenating the parts examples for branch names are: `feat/gh-104/profile-avatar`, `chore/gh-97/update-readme`, etc.

Do not use underscore (`_`) in branch naming, and don't use uppercase letters.
