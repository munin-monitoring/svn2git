## Moving Munin from SVN to GIT.

These collections of scripts are used to convert the existing munin
svn repository to git.

Existing tags are preserved

## Debian packaging

Existing Debian packaging branches are preserved as "packaging-*".

A new branch, "packaging-debian", is created to be used as base for
further packaging. It is merged from the latest tagged release, and
the "packaging-wheezy" branch.

To build packages, use "git-buildpackage" or "gitpkg" in this branch,
and set upstream-branch to "master".

There is no intended support for rebuilding historic debian packages,
these should be built from the archived SVN repository.
