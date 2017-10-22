# GitHub Tutorial

_by Victoria Feng_

---
## Git vs. GitHub
* **Git** is a tool to manage your source code history; doesn't require Github. 
* **Github** store code in the cloud and visually track changes; requires Git.

**Github** is a website where you run **Git** and become into repositories or projects, while **Git** is a repository when you manage your codes.
**Github** runs in a command line. It have a basic workflow. In **Github**, you can create a directory (folder) or files. 
Once **Git** is initialized for version control, we call it a repository (repo). 
You will know more in **Initial Setup**.

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
1- Make sure on the bottom of the box, it says "**<(your username)>: ~/workspace**".   
2- Type in "**mkdir first-repo**". Next, type in "**cd first-repo**". Make sure they are all lowercase and never use any spaces, use dash (-).  
3- Type in "**git init**". "**Git init**" starts git in our directory, which is now called a repo for version control.  
4- Add a README file to the directory, first-repo. Type in "**touch README.md**".  
5- Open the README file. Type something in the file. Save, add, and commit change in present tense.
For example, "**git commit -m "create readme"**".  
6- Go back to github, go to the top-right corner, "**+**", and press "**New Repository**".  
7- Name your repository, "**first-repo**". The names always need to be match and create repository.  
8- Make sure on the top, it says "**SSH**". Copy and Paste the URLinto the box one at a time. Use "**git remote -v**" to make sure you push into the right repo.
[Here is a picture of it!](file:///C:/Users/user/Pictures/SEP%20Project%201.png)

---
## Workflow & Commands



---
## Rolling Back Changes