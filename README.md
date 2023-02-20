# Linux Shell Implementation in XV6

## Code and Report
Click [here](https://github.com/aashaykorani/XV6-shell/blob/main/shell.c) to see the code.

Click [here](https://github.com/aashaykorani/XV6-shell/blob/main/Shell-report.pdf) to see my report for this project.

## Part 1 - Command Execution
Implement basic command execution by filling in the code inside of the case ‘ ‘  blocking the runcmd function. You will want to look at the manual page for the exec(3) function by typing "man 3 exec" (Note: throughout this course, when referring to commands that one can look up in the man pages, we will typically specify the section number in parentheses -- thus, since exec is found in section 3, we will say exec(3)). 
Once this is done, you should be able to use your shell to run single commands, such as 
cs6233> ls 
cs6233> grep cat words.txt 

## Part 2 - I/O Redirection
Now extend the shell to handle input and output redirection. Programs will be expecting their input on standard input and write to standard output, so you will have to open the file and then replace standard input or output with that file. As before, the parser already recognizes the '>' and '<' characters and builds a redircmd structure for you, so you just need to use the information in that redircmd to open a file and replace standard input or output with it. 

## Part 3 - Pipes
The final task is to add the ability to pipe the output of one command into the input of another. You will fill out the code for the '|' case of the switch statement in runcmd to do this. 


