# github-branch-merge-strategy

## Pre-commit

This code prevents commits on the 'main' or 'staging' branches. Every time a commit is made, it's executed to validate if you're on an allowed branch.

## Configuration

First of all, you must clone this repository.

Now you need to configure your local GitHub environment. There are two ways of doing this:

1 - Configure for each repository: In this case, you have to navigate to the root folder of each repository and run the following code:
```bash
git config core.hooksPath github-branch-merge-strategy
```

2 - Alternatively, you can configure it globally by adding the '--global' flag to the command, and the configuration will be applied to every repository:

```bash
git --global config core.hooksPath github-branch-merge-strategy
```
