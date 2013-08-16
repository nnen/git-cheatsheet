Git Cheatsheet
==============

Links
-----

* [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)
* [Why your company shouldnt use Git submodules](http://codingkilledthecat.wordpress.com/2012/04/28/why-your-company-shouldnt-use-git-submodules/)

Commands
--------

### Reset

    git reset (--soft | --mixed | --hard | --merge | --keep) [-q] [<commit>]

* `--soft` - doesn't reset index not working tree
* `--mixed` - reset index, not working tree (marked for commit -> not marked)
* `--hard` - reset index and working tree (all chages are discarded)

Miscellanelous
--------------

### Pushing to Remote Repository

    git remote add origin repository-spec
    git push -u origin master

### Push Local Branch to Remote Repository

    git push -u repository-spec branch-name

### Checkout Remote Branch

    git fetch repository
    git checkout -b branch-name repository/branch-name

### Reset (Revert) a Single File

    git checkout filename

Or, in case there is a filename with the same name as one of the branches:

    git checkout -- filename

