------- Introduction -------
      ------o0o------
- This project will show the process of me learning and researching about Git.

***Steps of working with Git:
- Firstly, you need a GitHub account; go on github.com and sign up an account.
- step_1: checking your repository's status:
	$ git status
# this command will hep you checking your current repository's status (files, changes, commits).
- step 2: adding your changes to commit with GIT:
	$ git add filename
	exp: git add ReadME.txt
- step 3: commit your changes to your repository's history with a short message desbricing the updates:
	$ git commit -m "Your messages"
	exp: git commit -m "Create ReadME"
- step 4: checking your commit log on Git:
	$ git log

Bonus:
	$ git diff
#this command will help you checking the difference between your current file and how it was at your last commit!

	$ git rm --cached filename
#if you're accidently adding wrong any file and want to undo it, this command will resolve your problem.
	exp: $ git add dummy_file.txt //wrong file
	     $ git rm --cached dummy_file.txt

	     $ git rm --cached . -r
	//To remove everything and start again

	
	$ git reset
#reset your current

* Tips: after using $git log or $git diff, type q to exit the screen. Type h for help.

***Working with GitHub & remote
- When you put your project (programming, documents,...) on GitHub that copy lives on GitHub's servers. This will make it 
a "remote" repository because it is not on your computer, but on a server, "remote" somewhere else.
- By pushing your local (on your computer) changes to it, you keep it up to date.
- In this section, I will share what I've researched about GitHub & remote.

** Notice: you need to make sure your local repository's name and the remote's name are the same.
exp: you create a repository on your computer and named it git-study, then the name of its GitHub's repository
(remote's name) must be git-study.

- There will be 2 cases when we start doing a project with GitHub
+ The first one, we've already created a local repository and you want to pull some projects from some certain remotes.
	step 1: make sure local repository's name and remote's name are the same.
	step 2: Open terminal and go to your local repos and type:
		$ git remote add origin <Url from GitHub>
+ And in case of you've still not created a local repository yet, you can just go to your remote (Github), and clone it
onto your computer
	step 1: copy the url of the repository you want to clone
	step 2: open terminal and go to the directory you want to clone it, after that type:
		$ git clone <Url from GitHub>
- Push your work onto remote:
	$ git push <remotename> <branchname>
# this is the fast-push which mean there's only you working on that project and you can do whatever you want.

- Pull in changes:
	$ git pull <remotename> <branchname>
* Tips: if the bug: "refusing to merge unrelated histories" appeared, you can use this command:
	$ git pull <remotename> <branchname> --allow-unrelated-histories

***Forks and branches***
- When you start to work on a project with other people, you should make a workplace for your own and that is when branch
is needed. Create your own branch and start working!
+ How to create a branch
	- step 1: on GitHub, go to your project and create a new branch at your master branch (there is a button branch
on there)
	- step 2: back to your terminal, go to your working directory, and type:
		$ git branch <branchname>
# This will create a new branch on your local.
	- step 3: synx your new local branch with your new online branch.
		$ git checkout <branchname>
		+ To check what branch are you on, type:
		$ git branch
# This will show all of your current branches on your local.
And now, let's working!
