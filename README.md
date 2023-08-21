# github-branch-merge-strategy

## Pre-commit

This code prevents the commit on branch main or staging. Every time a commit is made, it's executed and validate if you're in an allowed branch.

## Configuration

First of all, you must clone this reporitory.

Now you must configure you local github, there's two of doing so:

1 - Configure each repository: In this case you have to go to the root folder of each repository and run the following code

´´´bash
git config core.hooksPath github-branch-merge-strategy
´´´

2 - You can configure it globally add the flag --global and the configuration you reflect in every repository


´´´bash
git --global config core.hooksPath github-branch-merge-strategy
´´´
