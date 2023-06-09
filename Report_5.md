# Lab Report 5 
## Debugging Scenario
**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

I am using VsCode on Windows 11

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. 
Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

[image](Terminal_error.png)
[image](TestListExamples.png)
[image](grade_sh_code.png)

I was expecting for it to have no compilation erros to occur, but some of the outputs don't look like what they are supposed to be. I can see that there is something going wrong with the `grep` command, but I don't really understand what is occuring. Also at the end, we can see that somehow the test passing, doesn't look remotely right. I expected atleast to get 0/1 tests correct, but that doesn't show. 

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

I don't belive I put any other command-line arguments, so I'm for sure theres just something wrong with the code itself.

## TA Response

From your code, I would definetly go over the spacing of the `grade.sh` file again. Sometimes the spaces between a bash commmand and an option or in your case the `-e` can change how the computer interprets the code. Also try to check on line 10 spacing and how the `!` interacts with the rest of the line after correcting the spacing.

[image](terminal done.png)

After fixing the spacing errors in line 10 and the lines that use `grep` the code functions as it normally should. The little spacing errors in my code really changed the output of my code.

## Reflection
