touch README.md  
git init  
git config --global user.name "uname"  
git config --global user.email "email"  
git add README.md  
git commit -m "first commit"  
git branch -M main  
git remote add origin https://github.com/rioter1/gittutorial.git  
git push -u origin main  

# add username "uname"  
# add password/token "token"  

# If you get an error when using persoanl access token (password has been disabled as a feature) as it is ssh based  
# go around that error, open .git/config, replace origin https with ssh  
# this will fix the error with PAT, now you will may get a permission error while pushing Permission denied (publickey)  
# git pull --rebase will NOT work to resolve this error  


# checks to see if existing ssh keys are present
ls -al ~/.ssh   
# copy the existing ssh key to clipboard  
cat ~/.ssh/id_ed25519.pub  
# add ssh key to your github account (copy paste from your system to your github account) 

#check ssh connection   
ssh -T git@github.com  
# Change your remote's URL from HTTPS to SSH with the git remote set-url command.  
git remote set-url origin git@github.com:rioter1/gittutorial.git  
# verify url change   
git remote -v  

# stage and snapshots
git reset filename #remove staged changes  
git restore --staged # does the same as above  

git diff --staged # gives the diff between added and commited file  

# what gets commited enters staging env

# branching and merging

git branch #lists branch  

git branch newname # creates a branch with name = newname  

git checkout newname # switches branch to new branch  

# to merge the work
# first checkout
git checkout main  
# then merge
git merge newname  




# 
 
