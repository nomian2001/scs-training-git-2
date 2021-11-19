# The progress
I run the below commands after clone the repository's assignment:

### I. Fetching to get all branch of original repository:
```
git fetch git@github.com:noothaithinh/scs.baitap.2.git
```

### II. Adding remote repository to push my own repository
```
git remote add tung git@github.com:nomian2001/scs-training-git-2.git
git branch -M master
git push -u tung master
git checkout origin/develop
git push tung
```

### III. Creating gitignore
```
git checkout tung/master
```
In this step, I created the file named ".gitignore", then adding the content such as: 
```
.env
tmp\
```
Then, I push it into github
```
git add .
git commit -m "update gitignore"
git push tung/master
```
### IV. Creating branch release
In this step I created a new branch from branch master.
```
git checkout -b release
git push tung
``` 
Then I pull request from branch **develop** to branch **release**. In this step, I fix the conflict by removing the content of file "conflict_3_4.txt" on the branch **release**. Finally, I pull request from **release** to **master**.

