#Git Hooks

##About
Git hooks are scripts that run at specific times while using Git. A common hook is the pre-commit hook, which is activated after the user runs `git commit` but before the actual commit is made. It can be used to validate code, cleanup files, and really anything else you can think of.

If you want to learn more about how useful hooks can be, I recommend reading [Why You Need a Git Pre-Commit Hook and Why Most Are Wrong](http://tech.yipit.com/2011/11/16/183772396/) by [Steve Pulec](https://twitter.com/spulec).

##How To
To use a hook, copy (or link) it into `.git/hooks/` at the root of a repository.

##Help
###General
For a list and descriptions of all hooks, run the following command in a terminal:

    $ git help hooks

###pre-commit
To commit changes without running the pre-commit hook, run:

    $ git commit --no-verify

You may want to use `--no-verify` if the hook catches an intentional print statement in a python file.
