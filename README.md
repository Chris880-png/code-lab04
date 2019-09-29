# code-lab04
i had a lot of trouble i tried hard
Lab - Odds and Ends
==========
Follow the instructions line-by-line.  

* Type in the commands as is, but ignore the beginning prompt.  
* Enter, tab, up and down are represented by <ENTER><TAB>,<UP> and <DOWN>.  
* "No output" or "nothing happens" are valid answers to any of the questions.
==========

==========
1. Open a new terminal window.
[NO OUTPUT]
----------
==========
2. In your home directory, start editing a text file called temp.txt using nano.

Write the command you used to do this below.
----------
$ touch temp.txt



==========
3. Open another terminal

[NO OUTPUT]
----------
==========
3. In this terminal, show (list) all running processes / programs.

Write the command that you used to do this, and the last two lines of output.
----------
ls

 Tracing/
 Videos/
then tried ps

    1323    1261    1323       9112  pty1      197609 20:47:38 /usr/bin/ps
     1261    1260    1261       4992  pty1      197609 20:39:06 /usr/bin/bash





==========
4. Run the same command, but look for a specific process.  (It's the version of the command that has | grep ...).  Look for the program that you started to edit a file, nano.

Write the command that you used to do this, and all of the output.
----------
$ ls -l temp.txt





==========
5. Stop (kill) the process that's called nano "temp.txt" by using the process id shown in the output of your previous command (first number after user name).

----------
kill8


==========
6. Go to your other terminal window.  What happened to nano?  What was the message on the screen?

----------
no message (blank)

==========
7. Close the terminal window that nano was in, and go back to the terminal where you ran ps.

[NO OUTPUT]
----------


==========
8. Now... using nano, create a shell script in your home directory called hello.sh.  It should contain the following text exactly:

#!/bin/bash
echo "hi there!"

Quit and save when you're done.

What command did you use to do this?
----------
./hello.sh.
$ echo hello.sh
hello.sh




==========
9. Change the permissions (modify) on hello.sh so that the *user* (u) can *execute* (x) it: 

Write the commands that you used to do this below.
----------
./hello.sh. 

==========
10. Run your script (hello.sh).

How did you do this?  What was the output?
----------
a lot of data, alot.

==========
11. Change to the root directory.  Try running your script again (hello.sh).  What was the output (if there's an error, write it out)?
----------

bash: cd: too many arguments
 
==========
12. Now trying using the full, absolute path to your script (that is, starting with /...).  What did you write in?  What did it do?
----------
i wrote /...).
i gave back bash: syntax error near unexpected token `)'

==========
13.  Go back to the directory that your hello.sh script was in.  What command did you use to change to this directory? 
----------
$ cd echo hello.sh


==========
14. Type in the following command:

echo $PATH

Write down the output of this command
----------
/c/Users/Michael/bin:/mingw64/bin:/usr/local/bin:/usr/bin:/bin:/mingw64/bin:/usr/bin:/c/Users/Michael/bin:/c/Program Files (x86)/Intel/iCLS Client:/c/Program Files/Intel/iCLS Client:/c/WINDOWS/system32:/c/WINDOWS:/c/WINDOWS/System32/Wbem:/c/WINDOWS/System32/WindowsPowerShell/v1.0:/c/Program Files (x86)/Windows Live/Shared:/c/Program Files/Intel/Intel(R) Management Engine Components/DAL:/c/Program Files/Intel/Intel(R) Management Engine Components/IPT:/c/Program Files (x86)/Intel/Intel(R) Management Engine Components/DAL:/c/Program Files (x86)/Intel/Intel(R) Management Engine Components/IPT:/c/Program Files (x86)/Intel/OpenCL SDK/2.0/bin/x86:/c/Program Files (x86)/Intel/OpenCL SDK/2.0/bin/x64:/c/Program Files (x86)/Skype/Phone:/cmd:/usr/bin/vendor_perl:/usr/bin/core_perl


==========
15. Type in the following command to show all environment variables:

env

Write down the last two lines of output for this command
----------
.0/bin/x64:/c/Program Files (x86)/Skype/Phone:/cmd
_=/usr/bin/env



==========
16. Set your PATH to include your home directory.  Do the following (substituting student or username for professor)

PATH=$PATH:/Users/professor

Now check your path again.

echo $PATH

Write down the output of the last command.  It should include your home folder.
----------
$ echo $PATH
/c/Users/Michael/bin:/mingw64/bin:/usr/local/bin:/usr/bin:/bin:/mingw64/bin:/usr/bin:/c/Users/Michael/bin:/c/Program Files (x86)/Intel/iCLS Client:/c/Program Files/Intel/iCLS Client:/c/WINDOWS/system32:/c/WINDOWS:/c/WINDOWS/System32/Wbem:/c/WINDOWS/System32/WindowsPowerShell/v1.0:/c/Program Files (x86)/Windows Live/Shared:/c/Program Files/Intel/Intel(R) Management Engine Components/DAL:/c/Program Files/Intel/Intel(R) Management Engine Components/IPT:/c/Program Files (x86)/Intel/Intel(R) Management Engine Components/DAL:/c/Program Files (x86)/Intel/Intel(R) Management Engine Components/IPT:/c/Program Files (x86)/Intel/OpenCL SDK/2.0/bin/x86:/c/Program Files (x86)/Intel/OpenCL SDK/2.0/bin/x64:/c/Program Files (x86)/Skype/Phone:/cmd:/usr/bin/vendor_perl:/usr/bin/core_perl:/Users/professor

==========
17.  Go back to root (/)

Try running your script simply by typing

hello.sh

It should work now!  What is the output?
----------
bash: rd: command not found


==========
18.  Save this file in the repository that you created from parts 1 and 2.

Add and commit it to your local repository and push to the remote repository.  Check github to see that your work was submitted.
----------


==========
19.  Optional - Try writing this shell script!

In your repository, create an executable shell script called make_5_files that creates 10 files in the directory that it's called in.  The file names should be:
myfile1.txt
myfile2.txt
.
myfile10.txt

Use a for loop to do this.  Add and save in your repository, push to the remote.
----------


==========
20.  Optional - Try writing this shell script!

In your repository, create an executable shell script called say_twice.  It should take one argument - a filename.  It will cat out the contents of that file twice, with a row of dashes between each (use cat, echo... then cat again).  Create a test file calle foo.txt ... that contains foo, bar and baz... each on separate lines.

Add and save in your repository, push to the remote.

----------
