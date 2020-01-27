# How To Git

This doc is far from complete. PR this if you find a good resource that would be helpful to link here.

## Vocabulary 

* `git` repositories stores revision history for a group of files
* `git clone` makes a _complete_, *standalone*, _ful_ copy of a git repository. 
* git repos may optionally have lists of `remote`s -- urls that point to the location of other copies of ostensibly the same repository
* copies of git repos can get out of sync, so git lets you `git fetch` a repository at a `remote` location, and optionally `git merge` that repo's revision history into another git repo's revision history.
* `git pull` is just shorthand for `git fetch && git merge`
* `fork`ing is a github contrivance. Remember that `git` is entirely separate from but integral to `github`. If you `fork` a github repository, what happens is a copy of that repository is cloned into your own github account. You can `git clone` _any_ repository and it's basically the same thing, except that the clone doesn't necessarily end up on github.
* you can use `git bash` commandline tools to clone a github git repo down to your own machine. If you do so, you are not forking -- you are just cloning. When you clone, a link-back to the `remote` url is stashed in `.git/config` file, which you can see by running `git remote -v`. You can push changes back up to your github repo by running `git push` from your local clone.
* Github Desktop application is just a nice user-interface to `git` command-line tools.



## how to pull upstream changes

(Here's how to do it with `git bash`](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork)

clone your fork > branch menu > merge into current branch > select upstream/master. Perhaps before you do that, click the fetch button to make sure that your local clone is up-to-date with upstream.

then, push your local clone to github.

tada!

If you wanted to pull upstream changes from the class repo down into your fork, you would:

1. fork my repo
2. clone your fork to your local machine using either `git bash` tools if on windows or just `git` on mac, or using `Github Desktop` on either
3. on your clone -- `fetch` the `upstream` remote state, which will update your local remote-tracking `upstream/master` branch which you didn't know you had
4. Then, on your clone, `merge` the `upstream/master` branch into your clone's `master` branch
5. Then, `push` your local clone's changes up to your github copy (up to your fork).

You can do the above either with git bash https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork or with github desktop (see first post in this thread)
