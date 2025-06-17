## Folder Structure Example

    Group-Project-Showcase/
    ├── .gitmodules
    ├── README.md
    ├── CONTRIBUTING.md
    └── projects/
        ├── GroupProject1/ (submodule)
        ├── GroupProject2/ (submodule)
        └── GroupProject3/ (submodule)
        

## Logic Flow

This diagram shows the general structure and workflow for organising group projects in Git and GitHub. ReDI School maintains the `main repository`, while each student or group has their own *separate* project repository on GitHub.

![alt text](Assets/logicmap.PNG)

1. Student clones the ReDI School's repository to their computer using VS Code.
2. The students creates a new branch in the school repository for their project.
3. Inside their branch, the student **adds their own project as a submodule**, linking to their GitHub repo. 
4. Once the student is happy with the setup, they **push their branch to GitHub** and **create a pull request**
5. ReDI School reviews the pull request and, if everything looks good, **merges it into the main branch.**