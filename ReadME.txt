Steps of working with Git:
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