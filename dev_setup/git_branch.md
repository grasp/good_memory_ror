##reference
[摘自](https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches)


Create the branch on your local machine :

$ git branch name_of_your_new_branch  
Push the branch on github :

$ git push origin <name_of_your_new_branc  
Switch to your new branch :

$ git checkout name_of_your_new_branch  
When you want to commit something in your branch, be sure to be in your branch.

You can see all branches created by using  

$ git branch 


generate git sshkey
------------
https://help.github.com/articles/generating-ssh-keys  

some trick
-----------------------------
http://stackoverflow.com/questions/6565357/git-push-requires-username-and-password  

A common mistake is cloning using the default (HTTPS) instead of SSH. You can correct this by going to your repository
, clicking the ssh button left to the URL field and updating the URL of your origin remote like this:  

 git remote set-url origin git@github.com:username/repo.git
 
 after that , you need run  
 ssh-add
 
 git push orgin dev00
