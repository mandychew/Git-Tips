# Git Tips
Useful tips for collaborating on GitHub  

Here are some tips for when multiple people are collaborating on the same GitHub repository:

## 1. Try to avoid multiple people editing the same file. 
Can split a program into multiple files (in the main program file, can call functions from the multiple files)

## 2. Avoid editing files directly from GitHub website
In the event that multiple people must edit the same file, I recommend to edit files through local repository instead of editing files directly on the GitHub website. You can do so by cloning the repository to GitHub Desktop, and editing files through your local repository.
Explanation:
Con of editing on GitHub website:
When multiple people edit the same file concurrently, only the person who made the last commit will be saved. The other commits made by others will not be reflected on GitHub. If this mistake was made, the unsaved commits made by the other people can be accessed in the file's history on GitHub.
Why does this happen? 
Possibly because when editing files directly on GitHub website, it is editing the file that's in the cloud. Whereas when editing a cloned file, it is only editing your copy of the file, and other people have their own copies of the file.

Whereas when editing files on GitHub desktop (cloned repository) will ensure that the multiple people editing a file won't lose any person's changes. 
need to commit and then push to the cloud

## References
https://www.quora.com/Should-two-people-work-on-the-same-file-at-the-same-time-on-Git
https://stackoverflow.com/questions/4028845/how-two-people-concurrently-editing-the-same-file-is-handled
