# simplilearn-m-theta-tech-project
Demo for M-theta Technology Solutions ( Simplilearn ) 

**Steps to perform:**

- Start with the Production branch (master branch), and then create a HotFix  and Integration branch
- Subsequently, create Feature 1 and 2 branches that integrate to the Integration branch as shown in the above figure
- Commit some changes in the Feature 2 branch and merge it into the Integration branch. Delete this branch once merging is complete
- Commit some changes in the Feature 1 branch and rebase it to the Integration branch
- Merge the Integration branch into Hotfix and Production branch to update these branches
- Commit some changes in Feature 1 branch, and then merge it into Integration, Hotfix, and Production branch. Delete this branch once merging is complete
- Commit some changes in the Hotfix branch and merge it into the Production as well as the Integration branch

**Soultion:**

- Step 1: 
    - Login into the Github Account with your credentials. 
    - Create a new reporistory, add a Repository name to your project which yet to created 
    - It is a good practice to Add a README file into you reopsitory, by clicking on the checkbox we can create a README
    - It also good to add Add .gitignore, by clicking on the checkbox we can create a .gitignore
    - Now, click on create repository
- Step 2:  
    - As repository is created, now we need clone the project into our local machine using below command
        - `git clone https://github.com/vivekreddy0808/simplilearn-m-theta-tech-project.git`
    - Now it's time to check what Production is pointing to main or master branch
    - To check which branch the production is pointing to use the below command 
        -   `git branch`
    - If it's main branch, then switch it to master branch by using below command 
        - `git branch -m main master`
        - `git fetch origin`
        - `git branch -u origin/master`
        - `git remote set-head origin -a`
    - Once the Master branch is created for production now, it's time for us to create a HotFix and Integration Branch for future changes
    - Command to create a Hotfix and Integration (Using Integration branch --> Release branch)
        - `git checkout -b hotfix`
        - `git checkout -b release`  
- Step 3: 
    - As we need to add new changes, we create the feature branches according. 
     - Commands to create feature branches
        -  `git checkout -b feature-01`
        -  `git checkout -b feature-02`
-  Step 3.1: 
    - Now, it time to add some changes to feature branches, 
        - `create a new files into Feature-02 & commit the changes and merge it into Integration/Release branch`
        - `create a new files into Feature-01 & rebase into Integration/Release branch`
- Step 4:
    - Now, on the final step we check on the process of merging, commiting, updating & deleting the braches according the project requirement
