echo README.md  
git init  
git config --global user.name "rioter1"  
git config --global user.email prateek.gsharma@gmail.com  
git add README.md  
git commit -m "first commit"  
git branch -M main  
git remote add origin https://github.com/rioter1/gittutorial.git  
git push -u origin main  
username rioter1  
password/token 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  
# you will get an error when using persoanl access token as it is ssh based  
# to go around that error, open .git/config, replace origin https with ssh  
# this will fix the error with PAT, now you will get a perission erro while pushing Permission denied (publickey)  
# git pull --rebase will NOt work to resolve this error  
ls -al ~/.ssh # checks to see if existing ssh keys are present  
# copy the existing ssh key to clipboard  
cat ~/.ssh/id_ed25519.pub  
# add ssh key to your github account  
#check ssh connection   
ssh -T git@github.com  
# Change your remote's URL from HTTPS to SSH with the git remote set-url command.  
git remote set-url origin git@github.com:rioter1/gittutorial.git  
# verify url change   
git remote -v  

