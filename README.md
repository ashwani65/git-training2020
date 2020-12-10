# git-training2020

# Major Used Commands


## 1) Git Three Stage Architecture

<img alt="C++" width="500px" height="500px" src="https://static.packt-cdn.com/products/9781782168454/graphics/8454OS_01_4.jpg" />
<br/>

## 2) Tracking Git Projects

1) <b>git init</b>  (Make current Dir and Git Dir)<br/>
2) <b>git status</b> (To see the current status of dir)<br/> 
3) <b>git add "filename.extension"</b><br/>  
4) <b>git add --a Or git add . </b><br/>
5) <b>git commit -m "commit message"</b> <br/>
6) <b>git log</b> (To view the commit hisotry)<br/> 
7) <b>.gitignore</b>  (Include files and dir which you don't want to stage)<br/> 
8) <b>rm -rf .git</b> (Make curr dir and non-git)<br/> 
9) <b> git commit -a -m "message"</b> (Skipping the Staging area) <br/> 

## 3) File Status Lifecycle

<img alt="C++" width="500px" height="500px" src="https://git-scm.com/figures/18333fig0201-tn.png" />
<br/>

## 4) Git Diff : Changes b/w Staging area and Working Dir

1) <b>git diff</b> (Compare working dir with Staging area)<br/> 
2) <b>git diff --staged</b> (Changes to the files in Staged area)<br/> 

## 5) Moving and Renaming Files in Git

1) <b>git rm -file_name</b> (Removes and Staged)<br/> 
2) <b>git mv file_name renamed_filename</b> (Renames and moves to Staging area)<br/> 
3) <b>git rm --cached</b> (untrackes the file)

## 6) Git Log : Viewing and Changing commits in Git

1) <b>git log -p </b> (Log with diff)<br/>
2) <b>git log --stat</b> (log in Short) <br>
3) <b>git log --pretty=online </b> (Shows all commits with their hash)<br>
4) <b>git log --=2.days/2.weeks/2.months </b> (Will show commits from last time specified)<br> 
5) <b>git log --pretty=format:"%h --%an" </b> (There are many formats which you can play with)<br> 

## 7) Unstaging and Unmodifying Files

1) <b>git restore --staged file_name</b> (Staged to unstaged)<br/> 
2) <b>git checkout --file_name </b> (to unmodify changes)<br/> 
3) <b>git checkout -f </b> (Back to previous commit,will take you to the previou commit stage)<br/> 

## 8) Remote Repository

1) <b>git remote</b> (Will show if this Dir is remote or not)<br/> 
2) <b>git remote add origin "url"</b> (will add git url as Remote repo,and now your url will be the origin)<br/> 
3) <b>git remote -v</b> (Will show two urls for push ,pull)<br/> 
4) <b>git push -u origin master </b> (will push the files to the master branch of our remote repo)<br/>


## 9) SetUp SSH Key

1) <b>ssh-keygen -t rsa-b 4096 -c "email"</b> <br/> 
2) <b>eval $(ssh-agent -s)</b><br/> 
3) <b>ssh-add ~/.ssh/id-rsa</b><br/> 
4) <b>tail ~/.ssh/id-rsa.pub</b> (Copy SSH Key and Paste on the SSH Key Setup in Settings tab your profile)<br>

## 10) Setting Alias in Git

1) <b>git config --global alias.st status</b><br>
2) <b>git config --global alias.ct commit</b><br>
3) <b>git config --global alias.unstage "restore --staged"</b><br>

## 11) Creating and Switching Branches in Git

1) <b>git checkout -b newBranchName</b> (Changes in One Branch won't reflect on other branch) <br>
2) <b>git checkout master</b> (Will Switch to master branch) <br>
3) <b>git checkout branch1</b> (Switch to other branch "branch1) <br>
4) <b>git branch </b> (will show the current branch you are on)<br>

## 12) Branching and Merging

1) <b> Whenever you are switching the branch make sure you have commited that (Clean state is recommended)</b><br>
2) <b> git merge branch_name</b> (Will merge the current branch with the master  ,here you need to handle merge conflict also)<br>
3) <b> git branch -v</b> (info about the branch commits)<br>
4) <b> git branch --merged</b> (will show the already merged branch)<br>
5) <b> git branch --no-merged</b> (Will show the branch which are not merged yet)<br>
6) <b> git branch -d branch_name </b> (Deletes the specified branch ,Gives error if branch_name is not merged)<br>
7) <b> git branch -D branch_name </b> (Delete boths weather it is merged or unmerged branch

## 13) Pushing Branches to Remote Repo

1) <b>git push origin branch_name </b> (The branch you are pushing ,make sure you are on that branch only,when we push master branch,other branches does not get published)<br>
