# frequent-git-commands

Cheat sheet for git commands I constantly find myself having to look up over and over.

[Set Up Git](https://help.github.com/articles/set-up-git/)

[Git Documentation](https://www.kernel.org/pub/software/scm/git/docs/)

### Remove local branch.

`git branch -d the-local-branch`

### Remove all merged local branches.

_Note the branches `master`, `staging`, and `develop` are omitted from deletion._

`git branch --merged | egrep -v "(^\*|master|staging|develop)" | xargs git branch -d`

### Checkout a remote branch.
`git checkout --track origin/branch-name`
