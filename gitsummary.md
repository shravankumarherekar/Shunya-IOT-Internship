# **WHAT IS GIT?**
![](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2016/11/Git-In-Devops-What-Is-Git-Edureka-2.png)
**Git is a distributed version control system (VCS),for tracking changes in computer files.
It helps  establishing coordination between multiple developers,it facilitates with functions like who made what changes and when, it allows to revert back at anytime etc.**
> CONCEPTS OF GIT 
1. keeps track of code history
2. takes "snapshots" of your files
3. you decide when to take a snapshot by makng a "commit"
4. you can stage files before commitng

# **GIT BASIC WORK FLOW**

Git has three stages in which files can reside in ,viz. modified , staged and committed
1. modified-changed the file but have not comitted to repo yet
2. staged -marked a modified in its current version to go into next snapshot
3. committed-data is safely stored in local repo .

At one time there are 3,**4 different trees **of software repository present namely:

1. *workspace*: all changes we make via editors is done in this tree repository
2. *staging*:   all the staged file go into this tre of repository.
3. *local repository*: all committed files go to this repository
4. *remote repository*: this is the copy of local repository but stored in some server on internet.All the changes made in local repositor are not   directly reflected into this tree , but we have to push the changes to the remote repository
<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png" height="500" width="700" align="centre">  




# BASIC commands for git:

1. Configuration: To configure git in machine.
> $ git config  --global user.name 'name-of -the-user'
> $ git config --global user.email 'email-id'

2. Initialize: To create .git directory in machine.
> $ git init

3. Clone: Cloning the remote repo to local repo.    
> $ git clone (link-to-repo)

4. Status: To check the status of files in staging area.  
Check the status of files in staging area.
> $ git status <this will show either files are staged or committed>

5. Add: To add the files to staging area.  
To add the files to the staging area.
> $ git add . <this dot will add all the files to staging area.>

6. push: To push the file from local repo to remote repo.
 $ git push origin <branch-name>      # push changes into repository


[**documentation by kasab shravan kumar**](https://gitlab.com/K_shravan_kumar)
