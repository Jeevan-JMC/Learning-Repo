Here is a comprehensive Git and GitHub Cheat Sheet in Markdown format. Git is the tool you use locally on your computer, while GitHub is the website where you host your code. 
GeeksforGeeks
GeeksforGeeks
🛠️ Git: Essential Local Commands
These commands are used in your terminal to manage your project's history. 
The GitHub Blog
The GitHub Blog
 +1
Command 	Description
git init	Initialize a new local Git repository
git clone [url]	Copy a remote repository to your computer
git status	Show the state of the working directory and staging area
git add [file]	Add a specific file to the staging area
git add .	Add all new and changed files to staging
git commit -m "[msg]"	Save a snapshot of your staged changes with a message
git log --oneline	View a brief history of your commits
git branch	List all local branches in the current repository
git checkout -b [name]	Create a new branch and switch to it immediately
git merge [branch]	Merge a specific branch into your current active branch
🌐 GitHub: Remote Synchronization
These commands connect your local computer to your GitHub account. 
DEV Community
DEV Community
 +1
Command 	Description
git remote add origin [url]	Connect your local repo to a remote GitHub repo
git push -u origin [branch]	Upload local commits to GitHub (and remember the branch)
git push	Push changes to the already linked remote branch
git pull	Fetch and merge changes from GitHub to your local machine
git fetch	Download changes from GitHub but do not merge them yet
🚀 GitHub CLI (gh commands) 
If you have the GitHub CLI installed, you can manage GitHub features directly from your terminal. 
GitHub Docs
GitHub Docs
Command 	Description
gh auth login	Authenticate your terminal with your GitHub account
gh repo create	Create a new repository on GitHub from the terminal
gh pr create	Create a Pull Request for your current branch
gh pr list	List open Pull Requests in the current repository
gh issue list	List open issues in the repository
gh repo view --web	Open the current repository's page in your browser
💡 Workflow Summary
git add . (Stage your work)
git commit -m "Your message" (Save locally)
git push (Upload to GitHub)
