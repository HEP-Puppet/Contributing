Naming of modules
============
Please make sure your puppet modules have a name that describes their function as concise as possible.
Examples can be found at https://github.com/HEP-Puppet.

Please also ommit to have 'puppet' in the module name as the organisation name already includes that bit.
This helps to keep the module names short.

Git Usage: Merging and Rebasing
===============================

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
