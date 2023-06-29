# Local repository
### Init repository
```bash
git init
```

### add new/modified file to stage (stage is a temp work stage to store you work)
```bash
git add filename
```
**add before commit**

### commit file 
```bash
git commit -m "comment on your work"
```
**Comment let you know what you have done and for easy checking**

### check current stage status
```bash
git status
```

### Check difference between different version of a file,check log/relog
```bash
git diff filname
git log
git relog
```
In log, you can find the commit_id for every commit and use to reset your file;

### Reset file which is not added
```bash
git checkout -- filename
```
This mean you pull the file from master to replace the file in your current work area;
If the file has add to stage, use git reset;

### remove file in git repository
```bash
git rm filename
```

# Remote repository (Github)
### Step to connect local repository with github
1. In your local computer 
```bash 
ssh-keygen -t rsa -C "e-mail address"
```
Copy the content of .pub to your github account's ssh key

2. Create new repository in github

3. Add your local repository to github
```bash
git remote add origin git@github.com:your-git-hub-account-name/your-repository-name.git
```
**origin** is the name of remote repository name

4. Connect your brach and push files to github at the first time
```bash
git push -u origin master
```
*-u* 

5. push committed changed to github
```bash
git push origin master
```

### check remote repository
```bash
git remote -v
```















