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
    Store all the changes of the index to a new commit. If no files are marked and none are add witj ```git add``` the following error message will be addressed:  
    >nothing to commit, working tree clean  

    *Example :* ```git commit -am "This is a perfectly good commit."```  
    *Doc link :* [GitHub](https://git-scm.com/docs/git-commit)   

* **Git push** :  
    *Usage :* ```git push  <REMOTENAME> <BRANCHNAME> ```  
    Allow to push commit made on a local branche (using ```git commit```) to a distant repository.  
    *Example :* ```git push windows gitHub_main```  
    *Doc link :* [GitHub](https://git-scm.com/docs/git-push)  
	
* **Git add** :  
    *Usage :* ```git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p]
	  [--edit | -e] [--[no-]all | --[no-]ignore-removal | [--update | -u]]
	  [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormalize]
	  [--chmod=(+|-)x] [--] [<pathspec>…​]```  
    Add files to the index for futur commit. Can be omitted if -a option is used in ``git commit``
    *Example :* ```git add file.txt```  
    *Doc link :* [GitHub](https://git-scm.com/docs/git-add)  

* **Git pull** :  
    *Usage :* ```git pull [options] [<repository> [<refspec>…​]]```  
    Remove untracked files from the working tree
    *Doc link :* [GitHub](https://git-scm.com/docs/git-clean)  


* **Git clean** :  
    *Usage :* ```git clean [-d] [-f] [-i] [-n] [-q] [-e <pattern>] [-x | -X] [--] <path>…​```  
    Allow to pull all the chnage from a distant repository. If no repository is specified, it will used the linked repository if anny (set using ```git push -u foo bar```).  
    Git pull is the same as doing ```git fetch``` the a ```git merge``` .  
    *Example :* ```git pull origin master```  
    *Doc link :* [GitHub](https://git-scm.com/docs/git-pull)  


![git_war](https://i.pinimg.com/564x/fa/9b/ba/fa9bba627b338331730168e13b70b935.jpg)