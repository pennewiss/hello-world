# hello-world
Hello World Repository

## Edits on GitHub account
This is an edit of the README file

- Login on Github
- Open a project ("repository")
- Edit files in the repository directly (with the web editor)
- Save changes to the file ("commit" changes)

## Edits remote (Mac)
This is an edit made remotely using the git command

### Setup version control (git) on local computer
- Install code editor (e.g. Visual Studio Code)
- Open Terminal window in VSC
- Generate and save SSH key: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/connecting-to-github-with-ssh
 - Generate SSH key: ssh-keygen -t ed25519 -C "mygithubemail@mymailprovider.com"
 - Authenticate SSH: $ ssh -T git@github.com 

### Download project files from gitHub ("clone repository")
- Download repository to local computer: 
 - Go to folder to download to: $ cd ..
 - Clone repository: $ git clone "git@github" 
 - Open folder in VS to see all files and folders of the repository: File > Open...

### Save changes 
- Make changes to local repository
 - Make changes to files (e.g. README.md)
 - Add new files (e.g. index.html) and folders
- Save local changes to gitHub (commit changes)
 - Let git search for all changes made to the local repository: $ git status 
 - Tell git to add all changes to ALL files to the commit (incl. newly created files): $ git add .
  - Tell git to just add changes made to specific files to the commit: $ git add README.md
  - Tell git to remove specifc files from the commit: $ git restore --staged index.html
 - Commit changes (and add message to commit): $ git commit -m "Commit name" -m "Description text"  