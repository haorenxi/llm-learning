I started by linking my local repo to the remote Github repo.Since finding a clear how-to access is quite messy online,i wrote steps bellow.

🚀**first step**
- prepare a Github account.
- add a new repository by clicking 'New' button,and add your repository name,choose visibility.
  - *WARNING*:you are not recommended to choose 'Add README; Add .gitignore; Add license' button,since we will build a repo in local.
- Finally click 'Create repository' button which lied at the bottom.

💻**second step**
- Switch back to the local system
  >我滴妈英文好难
- Add a new filter,and *open Git Bash here*.Now we can get a Git terminal.
- sooooooo we come to Environment Configuration step.

```bash
echo "# llm-learning" >> README.md
git init
git add README.md
git commit -m "xxx" #'xxx' means you can add some Modification notes.
git branch -M main #Ensure that your branch's name,it may not be 'main'
git remote add origin https://github.com/your Github name/reponame.git

#you can check if successfully connectted remote repo by below code.
git status

# if you have modified 
git add xxx #specific modified file
git add . #all of the modified file

#Commit changes to the local repository
git commit -m "describe info"


# Synchronise local file modifications to the remote repository.
git push origin branchname 
```

🎉 Congratulation!Now you have mastered basic fundamental methods for synchronising local and remote repositories,now let us learning together!
