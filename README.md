# git_cheatSheet

***

This *readme* is a non exhaustive chit-chat for some useful git command.

* **Git commit** :
    *Usage :* ```git commit [-a | --interactive | --patch] [-s] [-v] [-u<mode>] [--amend]
	   [--dry-run] [(-c | -C | --fixup | --squash) <commit>]
	   [-F <file> | -m <msg>] [--reset-author] [--allow-empty]
	   [--allow-empty-message] [--no-verify] [-e] [--author=<author>]
	   [--date=<date>] [--cleanup=<mode>] [--[no-]status]
	   [-i | -o] [-S[<keyid>]] [--] [<file>…​] ```
    Store all the changes of the index to a new commit. If no files are marked and none are add witj ```git add``` the following error message will be addressed: :
    >nothing to commit, working tree clean 

    *Example :* ```git commit -am "This is a perfectly good commit."```
    *Doc link :* [GitHub](https://git-scm.com/docs/git-commit)

* **Git push** :
    *Usage :* ```git push  <REMOTENAME> <BRANCHNAME> ```
    Allow to push commit made on a local branche (using ```git commit```) to a distant repository.
    *Example :* ```git push windows gitHub_main```
    *Doc link :* [GitHub](https://git-scm.com/docs/git-push)

* **Git pull** :
    *Usage :* ```git pull [options] [<repository> [<refspec>…​]]```
    Allow to pull all the chnage from a distant repository. If no repository is specified, it will used the linked repository if anny (set using ```git push -u foo bar```).
    Git pull is the same as doing ```git fetch``` the a ```git merge``` .
    *Example :* ```git pull```
    *Doc link :* [GitHub](https://git-scm.com/docs/git-pull)

