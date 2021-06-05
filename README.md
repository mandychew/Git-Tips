# Git Tips
Useful tips for collaborating on the same GitHub repository.  

## Table of Contents
[1. Avoid multiple people editing the same file](#1.-avoid-multiple-people-editing-the-same-file)  
[2. Clone repository to GitHub Desktop and edit files through local repository](#2.-clone-repository-to-github-desktop-and-edit-files-through-local-repository)  
[References](#References)

## 1. Avoid multiple people editing the same file 
When editing different files, there won't be any conflict when committing the file.

## 2. Clone repository to GitHub Desktop and edit files through local repository
Please avoid editing files directly on the GitHub website, especially when multiple people have to edit the same file. Instead, I recommend to clone the repository to GitHub Desktop, and edit files through your local repository.  

### Why?  
It's because when multiple people edit the same file concurrently *on the GitHub website*, only the person who made the last commit will be saved. The other commits made by others will not be reflected on GitHub.  
- For example, Alice and Bob are editing the same file (in the same GitHub repository) on the GitHub website.  
Alice commits her version first. When Bob commits his version, Alice's changes are not saved anymore, it only shows Bob's changes.  
- If this mistake was made, the unsaved commits made by Alice can be accessed in the file's history on GitHub/VS Code.  

On the other hand, editing files *on the cloned repository* won't lose any person's changes.  
Using the example of Alice and Bob again... 
- Alice commits and push changes to remote (GitHub website) first.  
When Bob commits and push changes to remote, GitHub Desktop will warn him that the file has been changed by Alice. GitHub Desktop won't allow Bob's commit to be pushed to remote until he fixes the conflict.  
Only after fixing the conflicts, can he commit the resulting file (with both Alice's and Bob's changes).
- To reduce the number of conflicts to fix when committing, it's recommended to do pull requests regularly (and before starting to edit a file).

For more details on editing files on GitHub Desktop (cloned repository), this [answer](https://stackoverflow.com/a/4028856/15951751) explains it well.  
  
To understand why there's a difference between editing on GitHub website and a cloned repository, check out this [website](https://www.quora.com/Should-two-people-work-on-the-same-file-at-the-same-time-on-Git).

## References
Tip 2:  
https://www.quora.com/Should-two-people-work-on-the-same-file-at-the-same-time-on-Git  
https://stackoverflow.com/a/4028856/15951751
