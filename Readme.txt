Git global setup
git config --global user.name "Administrator"
git config --global user.email "admin@example.com"

Create a new repository
git clone http://git.iceragem.com:8899/root/master_v8.git
cd master_v8
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

Push an existing folder
cd existing_folder
git init
git remote add origin http://git.iceragem.com:8899/root/master_v8.git
git add .
git commit -m "Initial commit"
git push -u origin master

Push an existing Git repository
cd existing_repo
git remote rename origin old-origin
git remote add origin http://git.iceragem.com:8899/root/master_v8.git
git push -u origin --all
git push -u origin --tags