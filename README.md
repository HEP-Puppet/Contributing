# How to contribute

## Getting Started

* Make sure you have a [GitHub account](https://github.com/signup/free)
* Submit a ticket for your issue, assuming one does not already exist.
  * Clearly describe the issue including steps to reproduce when it is a bug.
  * Make sure you fill in the earliest version that you know has the issue.
* Fork the repository on GitHub

### Git Usage: Merging and Rebasing


Read this article for an in-depth discussion on
`git best practices http://lwn.net/Articles/328436/`.

Try to keep your history as simple as possible. Avoid merges on private code 
unless there is a particularly good reason to. Instead of merging in ``<project name>/master``
to update your local branch use rebase. Merging in ``<project name>/master`` risks
creating criss-cross merges which means you can actually lose code if you're
not careful. Git's merging algorithm is actually quite dumb, so it's best to
keep it simple. 

See the project's network for a graphical view of the projects's entire history::

``https://github.com/HEP-Puppet/<project name>/network``

Let's all try our best to keep this graph as clean as possible.

## Making Changes

* Create a topic branch from where you want to base your work.
  * This is usually the master branch.
  * Only target release branches if you are certain your fix must be on that
    branch.
  * To quickly create a topic branch based on master; `git branch
    fix/master/my_contribution master` then checkout the new branch with `git
    checkout fix/master/my_contribution`.  Please avoid working directly on the
    `master` branch.
* Make commits of logical units.
* Check for unnecessary whitespace with `git diff --check` before committing.
* Make sure your commit messages are in the proper format.

## New Modules
Repositories for new modules can be either requested as an issue in https://github.com/HEP-Puppet/Contributing
or created on your own github page first and then transferred to HEP-Puppet.

### Naming
Please make sure your puppet modules have a name that describes their function as concise as possible.
Examples can be found at https://github.com/HEP-Puppet.

Please also ommit to have 'puppet' in the module name as the organisation name already includes that bit.
This helps to keep the module names short.


