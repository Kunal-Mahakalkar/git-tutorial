`git init` -> powers your folder to managed by git ,and initialize a new
 empty repositorys. it also creates a . git folder that also has all 
 the relavant logic to manage versions of your projets.

 `working area` -> there can be a bunch of files that are not handeled by git.
 it means that changes done or to be done in those files are not managed by git 
 yet . a file which is in working area isconsiderd to be not in the staging area . when 
 we do `git status`  we see bunch if `untracked iles`then this are actually called to be in working area.

 3. `staging area` -> what all files are going to part of the next version that we will create .
 this stagingarea is the place wherer  git knows what changes will be done  from the last version to the next version .

 4. `repository area` -> this area actually contains the details of all you prviously 
 registered version. and the files in this area, git already manages them  and knows their version history.

 5. `git add <file>`-> moves file from working area to stagingarea

 6. `git rm --cached<file>`-> moves file back from staging area to working area .

 7. `commit`-> commit is a particular version of the project .it captures  a snapshot  of the project 
 's stacked changes and creates  a version out of it.
 
 8. `git commit`-> registers staging changes to a commit.

 9. `git log`-> list down all the commits of the repositories .if you wanyt to exit out from the git log 
 prompt press `q`.

 10.`git restore <file>`-> it removes all files from the staging area to be commited .
 this can be useful , if we  did some  dirty pieces of code and now  no more want it .
 insted of deleting every change line by line we can restore last clean version .

 11. `git restore --stacked <file>`-> it removes files from staging area to working area . 
 this only works when changes are at staging area .

 12. `difference between git rm and git restore `-> if you want to move the who,le file back  to the
  untracked state , then we do git rm , otherwise if we just want to change 
 to be moved in working area or staging area then we git restore. 

 13.`git diff commit1 commit2`-> gives the difference betweemn all files changes between two commits.

 14> `git commit -m "<your commit message>"`-> if we want to avoid opening a text editor like vim/ nano 
 to add commit message we can use this following command .
 