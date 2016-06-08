# Git Command Summary

* __git init__ _initialise a repository_
* __git add <file>__ _add a file to the staging area_
* __git commit__ _commit changes to the repository_
	* __-a__ _automatically stage existing files_
	* __-m__ _add commit message directly_
* __ git log__ _show changes in commits_
* __git diff__ _compare repository with last commit_
* __git mv__ _rename files in filesystem and repository_
* __git rm__ _remove files in filesystem and repository_
	* __--cached__ _remove files from repository but not filesystem_
* __git clone__ _clone a remote repository_
* __git checkout <branchname>__ _checkout a new branch_
	* __git checkout -b <branchname>__  _create and checkout a new branch_
* __git push__ _push your committed changes to the remote repository_
	* __-u origin <branchname>__ _set the remote repository branch you want to commit to_