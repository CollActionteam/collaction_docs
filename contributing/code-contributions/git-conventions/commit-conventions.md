# Commit Conventions

To ensure our commit history stays clean, and can more easily be used for tracking, we follow some simple conventions that go hand in hand with our [branches naming conventions](https://github.com/CollActionteam/collaction\_app/blob/development/docs/CONTRIBUTING.md#branches).

The format for the commit title is: `<tag>(<scope>): <subject>`

The format for a commit with body and footer is:

```
<tag>(<scope>): <subject>
<newline>
<body>
<newline>
<footer>
```

A full example commit:

```
feature(user): add missing user repository method

Motivation: Ability to update the authenticated user was missing

Closes: #117 Relates: #132
```

#### Tag

The tag describes the type of work that was actually done in the commit. This can differentiate from the branch name which the commit comes from, in case something changed and the purpose of the commit is not the same as it was intended. Most of the times, the commit tag will be the same as the branch tag.

See example tags from the branch naming conventions section.

#### Scope

The scope is not required, in case the scope is specific then it should be added for clarity.

See [example scopes](branching-conventions.md) from the branch naming conventions section.

#### Subject

The subject should be a short description written in clear, imperative and present tense. Use keywords in present tense such as `update`, `change`, `modify`, etc.

Examples: `update text to fit ui copy`, `hide tabs on profile`, `show onboarding on first app open`, etc.

#### Body

Similar to the subject, always use imperative, present tense. The body can be used to present the motivation for the changes in the commit. The body is not a required part, similar to the scope!

#### Footer

The footer is used for referencing Github issues, and if the commit is related to one or more specific issues, they should be linked in the footer.

References to issues with Github are made by prefixing the issue number with `#`.

Often used examples: `Relates: #100`, `Closes: #97 Relates: #103`.

If the commit relates to multiple issues, you can repeat the keyword for any amount of times necessary: `Relates: #60 Relates: #69`.
