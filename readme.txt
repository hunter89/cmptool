
Tool for comparison between two branches for a particular project or set of projects.


The tool:

cmptool
diffv4.py
sample.html



Tool functionality:

>>>Takes input as locations of folder where the branches to be compared are initiallized and the project(s) for which the comparison is to be done.

>>>Sync down the project(s).

>>>Return an HTML file as output with the comparison of project.



Tool Flow Explaination:

>>>Initialize the branches in different folders.(use repo_init.sh)

>>>While comparing for a set of projects; create a file with the project names (each project name in a new line).

>>>Check the output in output.html file.




USAGE:

>>>first argument: folder location of branch 1.

>>>second argument: folder location of branch 2.

>>>third argument: name of project or name of the file containing list of projects.

>>>options: 

	-f or --filename:	takes project name(s) input from a file.
	-q or --quick:		does not sync down the projects just compares the git log (used when updated projects are already synced). This option cannot be used with -f option.




NOTE:

This tool is essentially a bash script; So be advised to use a bash shell.

Synced down all components of tool in the same folder.

Ignore warnings related to "readonly variable OLDPWD" (used a dirty hack that is why the warning). 

It is advisable to always run the program in screen as syncing down the projects may take time.    
