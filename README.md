# GitHub Tutorial

_by Victoria Feng_

---
## Git vs. GitHub
* **Git** is a tool to manage your source code history; doesn't require Github. 
* **Github** store code in the cloud and visually track changes; requires Git.

**Github** is a website where you run **Git** and becomes a repositories or projects, while **Git** is a repository you can manage your codes.
**Github** runs in a command line. It have a basic workflow. In **Github**, you can create a directory (folder) or files. 
Once **Git** is initialized for version control, the directory will say master next to it. 
You will know more in **Initial Setup**. ``(Please edit to actually talk about initializing in the inital setup)``

---
## Initial Setup
1. First, you have to go to this URl, www.github.com(https://github.com/). 
2. Once you're done creating your Github account, you have to go to top right corner, which is your profile icon.
After you click on it, you go to Settings. There is a left sidebar and go to the label called "**SSH and GPG keys**". 
Press "**New SSH key**" and title it "**cloud9**". 
3. Next, go to the URL, cloud9(c9.io). Go to top right corner to the gear icon.
Go to SSH keys tab and copy and paste the second SSH key into Github. Type "**ssh-rsa**". Then, add the SSH key from before.
4. Go to cloud9 tab and open "**github-learning IDE**". On the bottom, there is a box with tabs labed "bash" with your username. 
Type in "**ssh -T git@github.com**". After you enter it, it should show "Hi <(your username)>! You've successfully authenticated, but Github does not provide shell access".
If not, you probably made a spelling mistake. 

---
## Repository Setup
* Make sure on the bottom of the box, it says "**<(your username)>: ~/workspace**".   -
* Type in "**mkdir first-repo**". Next, type in "**cd first-repo**". Make sure they are all lowercase and never use any spaces, use dash (-).  
* Type in "**git init**". "**Git init**" starts git in our directory, which is now called a repo for version control.  
* Add a README file to the directory, first-repo. Type in "**touch README.md**".  
* Open the README file. Type something in the file. Save, add, and commit change in present tense.
For example, "**git commit -m "create readme"**".  
* Go back to github, go to the top-right corner, "**+**", and press "**New Repository**".  
* Name your repository, "**first-repo**". The names always need to be match and create repository.  
* Make sure on the top, it says "**SSH**". Copy and Paste the URL into the box one at a time. Use "**git remote -v**" to make sure you push into the right repo.  
[Image](https://www.evernote.com/shard/s738/sh/b151dfce-8de1-412d-a3b2-efe48d5e47b6/12540d7d03c5a6b2e2aabbc3507ffa83)  

---
## Workflow & Commands
 * **git init**: Creates a new repository.  
 * **git status**: Keeps track of files which have been edit since the last commit, color in red.
It also see which command is ready for commitment, color in green.
 * **git add file.ext**: Add the file(s) that's ready to be commited.
   * **git add .**: Add the current directory that have changes.
   * **git add --all**: Add all changes, including deleted files.
 * "**git commit -m "(short/specific message)"** ": Take a snapshot of changes.
   * "**git commit -a**": Commit any files you added and commit any files you've changed
 * "**git push**": To push commits on your local branch to your remote repository
 * "**git pull**": Fetch and merge changes on the remote server to your working directory
 * "**rm -rf .git**": Remove hidden files.
 * "**git log**": See past commits.
 * "**git diff**": See the difference(s) between current code and the previous changes
 * "**git clone**": Create a working copy of a local repository
 * "**git push -u origin master**": Send changes to the master branch of your remote repository
 * "**git add remote origin URL**": Connect to your local repository to a remote server and push to it
 * "**git remote -v**": List all currently configured remote repositories  
[Workflow](https://www.evernote.com/shard/s738/sh/ea43fe4f-16cf-4a94-9296-de37ddf747d4/03fe453854151f3c1fa6578020203848)

---
## Rolling Back Changes
 * "**git checkout - - <(filename)>**": Replace changes in your working directory with the last content in head
 * "**git fetch origin**": Fetch the lastest history from the server and point your local master branch
 * "**git reset --hard origin/master**": Fetch the lastest commits and changes from your server to your local master branch
 * "**git reset --soft HEAD~1**": Undo lastest commit
 * "**git reset HEAD~1**": Undoing uncommited changes
 * "**git reset --hard HEAD~1**": Undo lastest commit
 * "**git reset HEAD <(filename)>**": Undo adds
 * "**git log sha/q**": Either sha or q to get the commit to quit
 * "**git revert**": Undo changes on a public branch; Undo commited changes
 * [Git Revert Example](https://www.evernote.com/shard/s738/sh/d34e85bf-32b0-4af0-b187-b0f1bdf03385/efb76703afbdc5858bda65f8d16c3ce1)
   *  where a is the lastest commit
   * where b is the commit before that
   * where c is the 3rd lastest commit  
[Rollback Summary](https://www.evernote.com/shard/s738/sh/0d42b101-224d-4072-b152-04c10293f0f2/05bced06a70ee902f67dd17e8a29fc65)

---
## Collaboration
 * ***Forking***: Produce a copy of a repository to your Github account
 * ***Cloning***: Make a copy to your local repository and making it your own remote
 * ***Pull Request***: Offering changes to orginal project by making it better  
   * The Master of the repository can accept or deny your offers of changes  
[Collaboration Workflow](https://www.evernote.com/shard/s738/sh/a86ba871-432d-4e88-8351-bd38ae5c509e/12749a8a9e5763fb702164217cd857bf)
