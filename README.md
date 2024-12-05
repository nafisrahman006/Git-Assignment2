## Task Description
<h3> This project demonstrates the use of Git for version control, including branching, rebasing, and managing pull requests. The steps below detail how to perform the task and include the necessary Git commands.
</h3>

## Create a new directory and initialize it as a Git repository
```
mkdir GIt_Assignment2
cd GIt_Assignment2
git init
```

## Add a README.md file and provide a brief description

```
touch README.md
echo "Hello World" > README.md
```
## Make an initial commit with the README.md file

```
git add README.md
git commit -m "Initial commit: first commit"
```

##  Push the repository to a remote hosting service 
```
git remote add origin <REMOTE_REPO_URL>
git branch -M main
git push -u origin main
```

## Create and switch to the feature-1 branch

```
git checkout -b feature-1
```
## Make changes and commit them in feature-1

```
echo "feature 1 file overwrite" > feature1.txt
git add feature1.txt
git commit -m "Added feature branch & file"
git push origin feature-1
Create a pull request for feature-1 merging into main.

```
## Switch to the main branch, create and switch to the feature-2 branch
```

git checkout main
git pull origin main
git fetch origin main
git rebase origin/main
git checkout -b feature-2

```
## Make changes and commit them in feature-2
```
echo "feature 2 file overwrite" > feature2.txt
git add feature2.txt
git commit -m "feature-2 branch added & add a new file"
git push origin feature-2
Create another pull request for feature-2 merging into main.
```



## After merging, check the commit history in the main branch
```

git checkout main
git pull origin main
git status
```
Delete merged branches locally and remotely

## Locally
```
git branch -d feature-1
git branch -d feature-2
```

## Remotely
```
git push origin --delete feature-1
git push origin --delete feature-
```
## Final Submission
```
git add README.md
git commit -m "Final Commit"
git push origin main

```