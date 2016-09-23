#Git Cheat Sheet

You want to...  
[Create a Pull Request](#anchor1)  
[Create Some New Stuff and Add to a Remote Repo] (#anchor2)  
[Undo Things!](#anchor3)  
[Check and Change the Current Terminal User](#anchor4)    

<a name="anchor1"></a>
##Create a Pull Request  
git clone [https address of repo] → Clones a remote repo into local directory  
git status → shows a log of changes  
git checkout -b [name of branch] → Branch the repo  
git add [changed files] → Stage changes. Changed files could be docs/style_guide  
git commit → commit the changes to the local branched repo  
git push origin [name of branch] → push the repo to the remote repo  
  
Check github for notification and create a pull request from the pushed change  
  
<a name="anchor2"></a>
##Create Some New Stuff and Add to a Remote Repo  
git init  
git status  
git add [changed files]  
git status  
git commit -m “describe what changed with this commit”  
git log → check the commit log  
git remote add origin [Repo URL]  
git push origin master  
git remote -v → shows you the URL that git has stored for the shortname to be used when reading and writing to that remote  

<a name="anchor3"></a>
##Undo Things! 
####Undo a "public" commit   
git revert <SHA> → Create a new commit that's the opposite of the specified commit  
git push → Need to push the new inverse commit  
####Undo a "local" commit  
git reset <SHA> → Undo the commit but keep the change on disk  
git reset --hard <SHA> → Undo the commit and revert the change on disk  
####Undo almost anything  
[How to undo almost anything with Git](https://github.com/blog/2019-how-to-undo-almost-anything-with-git)  

<a name="anchor4"></a>  
##Check and Change the Current Terminal User  
git config --list → Check the current user  





