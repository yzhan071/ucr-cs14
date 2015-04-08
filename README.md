# UCR CS 14 Spring 2015

**Submissions**

Your programming assignments will be submitted through GitHub. This is going to require that you learn how to use git. There plenty of help pages on the GitHub website that will walk you through the basics.

**GitHub**

You will need to sign up for a free account at [https://github.com](https://github.com). After creating your account go to [https://education.github.com/discount_requests/new](https://education.github.com/discount_requests/new) to an upgrade to a student account which will enable you to create private repos.

In order for your assignments you will need to create a private repository called "cs14_15spr" without the quotes. After creating the repository you will need to add me as a collaborator which allows me access to your files. To do this, go click on the repository settings button which is located on the right hand side of the page. On the next screen click the collaborators button and in the search box type in aguerrero and click the add collaborator button. Each assignment receive their own directory so assignment 1 files will be located in hw1, assignment 2 in hw2 and so on.

After you setup your account go to [https://github.com/aguerrero/ucr-cs14-15spr](https://github.com/aguerrero/ucr-cs14-15spr) and fork the repository. In your forked repository go to the students directory and create a file named as your UCR username. So if your UCR username is abcde012 you would create a file with that name. In the file include the following lines:

name = *First Last*

ghurl = https://github.com/*yourGitHubUsername*/ucr-cs14.git

After creating a this file with the required information push the changes to GitHub and make a pull request. Instructions on how to do this can be found on the GitHub website and by searching Google.

After you have worked on your assignment and are ready to submit you code you must first tag the work you want graded. For example, if you were submitting assignment 1 you would simply run ‘git tag hw1’. Tags don’t get pushed along with your other commits so you must explicitly run ‘git push --tags’ for your tags to show up on GitHub. If you update your code and already tagged your submission you can delete the old tag by running ‘git tag -d hw1’ ,creating a new tag with the same name, and then pushing to GitHub.

Tagging your submission is a very important step. When grading your work I will run the following commands:

git clone *address-to-your-repo*

git checkout hw1

You will receive a grade based on what you have tagged as hw1 so if nothing is tagged as hw1 you will receive a 0.

**Assignment Specification**

It is very important that you follow assignment specifications. Many of the assignment specifications will provide you with a set of functions that you must implement. It is important that the functions you implement have the same parameter type and return type as what is specified in the assignment description. Make sure you are naming your functions as specified as well.

I will be writing my own main.cc file to test your assingments. For example, in assignment 1 you are required to implement a function ‘void insert_at_pos(int i, char value)’. It is ok if you use variable names other than i and value but the rest of the declaration must stay the same. This means that ‘void insert_at_pos(int foo, char bar)’ is ok but ‘void insertAtPos(int i, char value)’ is not and will not receive credit.

**Compiling**

All of your programming assignments will be graded on hammer. In order to make sure that your program is gradable you will need to compile it yourself on hammer before submitting. In order to do this you will need to enable C++11 for GCC. To do this you must first log onto hammer by running ‘ssh *username*@hammer.cs.ucr.edu’ . Once logged in you must add the following line to your .bashrc.

source /opt/rh/devtoolset-2/enable

After you have added this to your bashrc run ‘. ~/.bashrc’. You now have C++11 enabled for GCC. When you compile your code you must use the following command:

g++ -std=c++11 -Wall -Werror -pedantic* filename*

This is the command I will be running to compile your code so if it doesn’t compile for you it will also not compile for me.

**Grading**

Your grade for an assignment will be based on code that I will be writing to thoroughly test your assignments. When you write your main.cc to test the rest of your code make sure that you test for edge cases that might break your code as these are cases I will likely test for.

**Important**

* Code that does not compile **WILL RECEIVE A 0.**

* Late penalty is 10% for each day late up to a max of 2 days. Early bonus is 3% for each day early up to a max of 2 days. "Day early/late” is defined as 24 hours before/after due time.

* If your code compiles but segfaults before anything can be tested you **WILL RECEIVE A 0.**

* If your code segfaults you will only have a chance to receive credit for anything up until that point.

