# Git onboarding

## Command Summary

### <u>clone</u>

The *clone* command is used to obtain a copy of a remote repository in your own device for the first time. With this command you get all the repository history and sets the basic working environment you need. This automatically creates a local repository, configures the remote repository as "origin", and checks the default branch.

### <u>pull</u>

The *pull* command is used to bring and apply all the changes made and uploaded to the remote repository into your local branch. This will bring new commits from the remote repository and integrate them into the current local branch. If you have local changes, you should commit or stash them before pulling the remote ones, this way you will avoid conflicts. You could see git pull as a two-command step:

```bash
git fetch
git merge # (or rebase)
```

where first it gets the remote changes and then applies them into your local repository.

### <u>fetch</u>

The *fetch* command is really similar to the *pull* one. The difference is that *fetch* only brings the remote changes into the local repository but does not apply them automatically. This way, the local knows that there are changes to be applied but waits for manual approval to include them in the local working branch. 

### <u>switch</u>

The *switch* command is used to move between branches in your local repository. It is important because once you create a new branch to work on a feature, you have to switch to it to work on the necessary changes. It does not merge branches or transfer commits between them, it only changes the current working branch.

### <u>diff</u>

The *diff* command is used to visualize all the changes made to different files in your local repository since the last commit. It will show what lines you deleted or added in all the modified files.

### <u>add</u>

The *add* command is used to select what files are being sent to the staging area. In other words, it selects what changes made to the files are going to be saved and then probably added to the remote repository in a specific branch.

### <u>commit</u> 

The *commit* command is used to save or "take a snapshot" of your code at a certain point. It is basically a checkpoint in the history of the project so you can go back if anything goes wrong or the team decides that everything has to return to a certain point.

### <u>push</u>

The *push* command is used to upload local commits to the remote repository. This ideally has to be on a branch that is not "main". Then you can create a pull request from the branch you pushed your changes to and then merge it into main, if approved. 

## Use cases

### 1. Clone repo, create and move to new working branch

```bash
git clone git@github.com:fire2a/C2F-W.git
cd C2F-W
git switch -c feature/api # origin/main can be added at the end of the command to be based on the remote
```

### 2. Obtain changes from remote/main to working branch

```bash
git switch feature/api
git fetch origin
git rebase origin/main
# Other files were modified locally after this process
git diff
```

### 3. Upload local changes

```bash
# While still being in the feature/api branch and having modified files without conflict:
git add .
git commit -m "add: api feature"
git push --set-upstream origin feature/api
```