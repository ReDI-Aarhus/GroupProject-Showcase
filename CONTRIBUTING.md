
# Contributing
Instructions for students or contributors how add their group project, branching naming rules etc. 

Naming Convention:
- Repository Folder:
    - year-season-projectname
- Branch Name:
    - year-season-projectname-yourname

*Request ReDI School to be a contributor to this Repo if you haven't been invited yet. Otherwise, you cannot create a branch from this repo*


## ✅ Step 1: Setup Your Own Repository
Folder name is formated to this naming convention: (e.g, `2025-spring-hangmangame` )
    
    year-season-projectname

    
## 📁 Setup Your Project Folder
Each `project` folder should contain:
- `README.md`: brief description of the project
    - small intro, goals, features, conclusions
- `.py`, `jpynb`, `txt` files: Python Code and Text
- Asset folder (optional)
    - images

*When your repo is complete, you are read to move onto ReDI's Repo to do the next steps*

## ✅ Step 2: Clone ReDI School's Main Repository in VS Code Terminal
On GitHub, click `<> Code` to copy the URL 

*Hint
: https://github.com/ReDI-Aarhus/Intro-to-Python-GroupProject-Showcase.git*

In VS Code Terminal write the `bash command`:

    $ git clone https://github.com/ReDI-Aarhus/Intro-to-Python-GroupProject-Showcase.git

## ✅ Step 3: Create a Branch from ReDI's Repo

In the same Terminal create a branch from `main` (e.g., `2025-spring-hangmangame-steph`):

    $ git checkout -b "year-season-projectname-yourname"
    $ git push -u origin year-season-projectname-yourname

## ✅ Step 4: Check your branch on GitHub
On GitHub, located on the near the top of ReDI's repository page, click the `Branches` tab to be sure your branch is in the repository

## ✅ Step 5: Add Submodules in Your Branch
In VS Code Terminal write the `bash command`

    git submodule add <repo-url> projects/yourrepofoldername

*Hint*
- Copy *your repo URL* into the following command (e.g, `https://github.com/StephSegaW/HangmanGroupProject.git`)
- specify to put it into the Projects folder

Example

    git submodule add https://github.com/yourusername/repoproject projects/HangmanGroupProject

## ✅ Step 6: Commit the Changes
After adding the submodule, Git creates a special file called `.gitmodules` and adds a reference to each submodule.

Write the following commands in bash to stage and commit your work

    git add .gitmodules projects/yourrepofoldername
    git commit -m "Add submodule projectname"

Then push:

    git push -u origin nameofyourbranch


# 📌 Best Practices

## 🔄 Pulling updates from Main to Your Branch
Check your branches status compared to main

    git status
    
This fetches changes from the remote main branch

    git pull origin main

You've made changes but not yet been pushed to the remote repo. Push the updates to your branch

    git push -u origin your-branch-name



## 🔄 Saving Changes in Your Branch
You may want to update your repository. You should save your work, stage it (add) and then commit (commit -m). Be sure to push your commit to your branch again after.

### ✅ Step 1: Save your changes
Always `SAVE` your changes in the file you modified. 

### ✅ Step 2: Stage and Commit your changes
    git add filename
    git commit -m "your comment description"
### ✅ Step 3: Push your commits to your branch
    git push -u origin nameofyourbranch

### ✅ Step 4: Check your branch it is up to date
Use the following to double check your last commit history and the status of your branch. You can use it before your start and after your push your work. 

    git log
    git status

