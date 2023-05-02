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


