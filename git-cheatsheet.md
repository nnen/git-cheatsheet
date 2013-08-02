Git Cheatsheet
==============

Commands
--------

### Reset

    git reset (--soft | --mixed | --hard | --merge | --keep) [-q] [<commit>]

* `--soft` - doesn't reset index not working tree
* `--mixed` - reset index, not working tree (marked for commit -> not marked)
* `--hard` - reset index and working tree (all chages are discarded)

Miscellanelous
--------------

### Push Local Branch to Remote Repository

    git push -u repository-spec branch-name

### Checkout Remote Branch

    git fetch repository
    git checkout -b branch-name repository/branch-name

### Reset (Revert) a Single File

    git checkout filename

Or, in case there is a filename with the same name as one of the branches:

    git checkout -- filename

