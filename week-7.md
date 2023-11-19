### Lab Report 4 - Vim (Week 7)
#### 4. Logging into ieng6

Screenshot: 

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/b7df2b7e-381b-4733-9ab1-dab27fc8a81d)

Keys pressed - I typed the following command and argument:
``` 
ssh cs15lfa23mb@ieng6.ucsd.edu
```
to log into my ieng6 machine
and then pressed `<Enter>` to run it

Command summary: `ssh` into the specific email allows me to log in to the ieng6 machine from a remote computer (my laptop).

#### 5. Cloning lab7 repository

Screenshot: 

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/972bc4b0-476f-4f0f-9140-6a4e768c027c)

Keys pressed: From the github repository page, I first copied `git@github.com:cnidyllic/lab7.git` to my clipboard and then `Ctrl-V` to paste it with the `git clone` command:
```
git clone git@github.com:cnidyllic/lab7.git
```
to clone my fork of the assignment's repository 
and then pressed `<Enter>` to run it

Command summary: `git clone` allows me to clone a repository by accepting a `<repository_url>` as an argument


#### 6. Running tests (before fix)

Screenshot: 

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/a44ca1e4-8981-4871-b8ac-8466ff475bbc)

Keys pressed: I first typed in the `cd` command and then typed `l` `<Tab>`, and then pressed `<Enter>` to run in the command line:
```
cd lab7
```
Then, I typed `bash` command, `t` `<Tab>`, and then pressd `<Enter>` to run in the command line:
```
bash test.sh
```

Command Summary: The first command and argument changed into the directory that I had just cloned called `lab7`, which I was able to access with one letter because I knew there was only directory 
under the `home` directory that started with an `l`. I was able to access `test.sh` in a similar way as well. The `test.sh` file contains the `javac` and `java` commands with the appropriate test libraries 
which allowed me to run the tests in this fashion.

#### 7. Editing the code file ListExamples.java

Screenshot (s) : 

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/9861ed0c-87b3-4a3a-a402-ec32288e5412)

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/45be1a11-7497-41d3-83a9-d9e81c41dcee)

Keys pressed: First, I typed in the the `vim` command then `<Shift>` `l` `<Tab>` `.` `<Tab>``<Enter>` to run in the command line:
```
vim ListExamples.java
```
Then in the file, I typed `43j`,`11l`,`r2`,`:wq` to fix the error.

Command Summary: When typing the `vim` command with the argument, I type the first letter of the file I wanted which was `L` and then tabbed to auto complete, since there were two files that had `ListExamples` 
in their file name, I had to press `.` and then another `<Tab>` to autocomplete again. While in the file, in the test run I checked the coordinates of the error that I wanted to fix at, which was `<44,12>`. Since
I started at `(1,1)` at the beginning, I had to move 43 lines down which is `43j`, 11 lines to the right `11l`, replaced the character `1` with `2` using `r2`, and then saved and exited the file with `:wq`.

#### 8. Running the tests (after fix)

Screenshot: 

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/d1a34d3c-d1ef-450d-8ef1-bd51000ddfe9)

Keys pressed: `<up><up><enter>` to run the same command as I did in Step 6.

Command Summary: The command that was run was run 2 commands ago, which is why I used the up arrow twice to copy it. The command functionality can be referred to in Step 6. 

#### 9. Committing and pushing Changes to GitHub

Screenshot:

![image](https://github.com/cnidyllic/lab-report-4/assets/146884284/68ee1051-134b-4013-aa3e-515225e7e56c)

Keys pressed: 
I first typed in the `git add` command and then typed `<Shift>` `l` `<Tab>` `.` `<Tab>``<Enter>` to run in the command line:
```
git add ListExamples.java
```
Then, I typed `git commit -m` command and option, with the message `"changed index1 to index2 in merge function:`, and then pressed `<Enter>` to run in the command line: 
```
git commit -m "changed index1 to index 2 in merge function
```
Finally, I typed `git push` command to push the new changes and message to my repository.

Command summary: In the first `git add` command, I used a similar short cut to get the `ListExamples.java` file name which I used in step 7 during `vim` command (you can refer to that for the explanation). Then I committed these changes using `git commit -m` with a relevant message summarizing the change that I made in the file. Finally, I pushed these changes with `git push` to the main repository `lab7` (not cloned).
