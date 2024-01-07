Exercise 02: Version Control
---

The goal of this exercise is to use git to control the source of a simple C++ application. While this exercise demonstrates the command line usage, you can also use one of the many GUI frontends or IDE extensions for git if you prefer. In my experience it is a good idea to at least be familiar with the basic command line usage.

GitHub Invitation URL

Prerequisites:

* You have completed Exercise 01: Setup and have a working command line with compiler and git accessible.
* If you are unfamiliar with the command line, you have gone through this crash course first.
* You have read through Chapter 1 of the Pro Git Book.

Steps:

1. One-time git configuration (skip if you have done this before). Open your command line and type the following (replacing the information as appropriate of course):

	```
	git config --global user.name "Your Name"
	git config --global user.email pid@vt.edu
	```
	
	You might also want to tell git what your preferred editor is for creating longer commit messages. For example on Windows, if you use Notepad++, you might type:

	```
	git config --global core.editor "'C:/Program Files (x86)/Notepad++/notepad++.exe' -multiInst -nosession"
	```
	
	Another popular cross platform editor is Atom(https://atom.io/). If you have installed it you can make it the default git editor by typing:

	```
	git config --global core.editor "atom --wait"
	```
 
2. Create a working directory somewhere on your computer. Open your command line terminal and make a working directory. Then change to that directory.

3. Clone the assignment for today. Accept the GitHub invitation at the link above. This will automatically add a repository accessible to you and the instructor/TAs with some starter files. You can then clone this to your computer using

	```
	git clone https://github.com/VTECE/ece3574-fl23-ex02-USER.git
	```
	where USER is your GitHub username. You may have to enter your GitHub username and password.

4. Change to the repository directory. Write a program in hello.cpp to print “Hello World!” to standard output.

5. Add the hello.cpp file to the index

	```
	git add hello.cpp
	```
	
6. Commit the change with a message
	
	```
	git commit -m "Added hello program"
	```
	
7. Use git log to see the results

	```
	git log
	```
	
8. Change the program to add another line of output “My name is NAME”, where NAME is your name.

9. Add the change to the index

	```
	git add hello.cpp
	```
	
10. Use git status to see the state of the repository

	```
	git status
	```
	
11. Commit the change with a message

	```
	git commit -m "Added my name."
	```
	
12. Use git log to verify the results

	```
	git log
	```
	
13. Use git push to synchronize the repository with that on GitHub

	```
	git push
	```
	
	You may have to enter your GitHub username and password again.

14. Use git tag to label the commit

	```
	git tag mylabel 
	```
	
15. Verify the tag is present

	```
	git log --decorate
	```
	or
	```
	git show mylabel
	```
	
16. Use git push to synchronize the repository with that on GitHub

	```
	git push origin mylabel
	```
	You may have to enter your GitHub username and password again.

17.	If you want to double check everything is pushed to GitHub you can check the repo in your browser.

18.	Post your git URL for Exercise 2 and the screenshot of "git log" to Canvas.

**This is how you will turn in exercises and project code in this course**, so be sure you understand these steps.

You have now completed the exercise.
 
