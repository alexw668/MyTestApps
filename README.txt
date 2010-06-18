Git Branching


o	List branch

		git branch
	
	The branch that's marked with "*" is the current one
	
o	Create a production branch

	git branch production
	
o	To switch to a specific branch

	git checkout [target branch]	
	
o	Merge into a branch 

	To merge current branch into a targeting (e.g., merge master into production):
	
	git checkout production
	git pull origin production         # to get latest from remote
	git merge master		
	
o	Push a branch to server

	git push origin prodution
	
	
	
Capstrano setting

set :repository, "git@github.com:vanpelt/rails-app.git"  # Your clone URL
set :scm, "git"
set :branch, "production"	(older version: set :branch, "origin/production")

	