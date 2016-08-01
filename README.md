# githooks
A small repo with some useful githooks

Currently there are hooks for `pre-commit` and `post-merge`. According to the [Git-hooks documentation](https://git-scm.com/docs/githooks):

> [The post-merge] hook can be used in conjunction with a corresponding pre-commit hook to save and restore any form of metadata associated with the working tree (e.g.: permissions/ownership, ACLS, etc).

Because we use MySQL and because the db schema often differs between branches, you can use these hooks to save/restore your branch's db schema.

You can configure your system to use git hooks from `~/.git/hooks/` (so you can download these hooks and put them there), or you can use the hooks an a per-project-basis. If you'd like to do it this way, put the files into `your/project/path/.git/hooks`.
