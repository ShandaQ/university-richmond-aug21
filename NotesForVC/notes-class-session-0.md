# Notes for Class Sessoion 0

## 1. Everyone Do: GitHub Activity  

1. Navigate to the GitHub website.
      
2. Create a new repository using the GitHub user interface.

3. Navigate the file system using the command line by typing `cd`, `ls`, and `pwd`.

4. Clone a repository using the `git clone` command.
    - want to naviagte to the project directory
    - **git init**
        - necessary repository filesl git repository skeleton 
        - ls -a list all the hidden files 

    - project you want to contribute to
    - get all the data... every file version gets pulled -> get clone
    - get clone <url>
        - clone into a directory name something else 
        - git clone https://github.com/ShandaQ/university-richmond-aug21 testing
        - cd into directory and open the .md file. 

5. Create a new file using the `touch` command.
    - cd into the directory 
    - touch testing.html

6. Push changes to the GitHub repository using the `git status`, `git add .`, `git commit -m "message"`, and `git push origin main` commands.
    - creating snapshots/ pushing changes to the repo when you are happy with the changes you have made
    - files have states
        - tracked (files that git knows about)
            - files in the last snapshot; early staged files
            - unmodified, modified, stages

        - untracked (everything else)
            - all files in working directory that are not in the last snapshot 
            - and not in staging area
            - **on first clone, all files are tracked and unmodified**
        **as you being to make changes to files git -> modified -> since they have not yet been commited**
        ### Cycle
        - untracked
        - unmodified
        - modified files 
        - stage modified files
        - commit staged changes
        - repeat
            
    ## Check status of files 
    - git status
        - will list Branch name -> master by default
        - and untrack files -> files that were not including on the previous snapshot/commit and have not been staged
        - you must treat git with special gloves and tell it what to do and when to do it
    
    ## Tracking Files 
    -   <file name>, git add . -. all files in given directory
    - git status

    ## commiting Your Changes
    - **anything that you did not run a git add on since an edit was done will not go into this commit**
    - git commit -m "first commit' **records the snapshot of staging area**
    - snapshot can be used to revert back to or compare
    - git commit -a -m 'adding a -a in the git commit lets you skipp the git add step, auto stage every file that is already being tracked'

    ## Push changes to remote repo
    - git push origin main -> push local changes to oline repo
    - git status


    **Extras**
    ## View Stage and Unstage Changes
    - git -diff answers
        - what was changed but not staged
        - what was staged but not commited
        - git diff shows lines added and removed
        - git diff to see the changes in the file that are staged and the changes that are unstaged.
    
    ## Removing Files
    - must remove from tracked file aka staging area and then commit
    - **rm <file name> does the above plus removes the file from working directory
        - status -> changes not staged for commit
    - ** git rm <file name>
        - it stages the file removal
    - run git commit -> file gone and no longer tracked
    - if the file has been modifed, use -f to force the removal 

    ## Moving Files
    ## Unstaging
    ## Unmodifiing 