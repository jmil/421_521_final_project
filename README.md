#Bioe 421/521: Microcontroller Applications
####Instructor: Jordan Miller<br>TA: John Sexton<br>github.com/jmil/Bioe421_521-MicrocontrollerApplications

# Final Projects


This `git` repository is a super repo holding all class projects, giving a global view of class progress.

First clone this super repo:

	$ git clone git@github.com:jmil/421_521_final_project.git
	$ cd 421_521_final_project

Next we tell the repo to notice that it has submodules that are referenced. Wake up each one, and checkout the commit referenced with the given checksum.

	$ git submodule init
	$ git submodule update
	

Later, to traverse all submodules and pull down latest versions you run:

	$ git submodule foreach git pull origin master

If changes were pulled down, don't forget to update the master branch of this super repo by committing the latest commit references for each submodule.

	$ git status
	$ git add .
	$ git commit -a -m "submodule XXX updated"
