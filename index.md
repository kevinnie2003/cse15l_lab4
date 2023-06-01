# Step 4: Log into ieng6
```
$ ssh cs15lsp23cx@ieng6.ucsd.edu
<enter>
```
The reason for not needing to enter a password is that I have generated a SSH key for ieng6.

When I log in from my local computer, I won't be prompted for a password.

Here is the link from the course website that introduces how: 

https://ucsd-cse15l-s23.github.io/week/week7/#generating-ssh-keys-for-ieng6

<img width="945" alt="截屏2023-05-17 18 29 49" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/a0ee3b74-2389-4d0f-8171-09e30fada609">

# Step 5: Clone your fork of the repository from your Github account
```
$ git clone https://github.com/kevinnie2003/lab7
<enter>
```
<img width="675" alt="截屏2023-05-17 18 36 05" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/688b2c62-9868-4b9e-b35d-8ecec0976cb7">

# Step 6: Run the tests, demonstrating that they fail
```
Keys pressed: cd lab7 <enter>, bash test.sh <enter>
```
<img width="729" alt="截屏2023-05-17 18 37 15" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/643df8f3-f47b-4d2b-be46-ccf05094552d">

# Step 7: Edit the code file to fix the failing test
**There are two bugs. Here are the keys pressed to fix them one by one.**
```
Keys pressed: vim L <Tab> T <Tab> <enter>
```
Tab allows users to quickly navigate through the system and execute commands without typing the full name of the command. 

By pressing Tab, it can automatically complete a partially typed file or command name.

In our case, this is the same as "vim ListExamples.java"

Now editing the file ListExamplesTest.java.
```
<esc> 100k 100h 11j 75l r2 4l r1 :wq <enter>
```
Pressing esc allows us to make sure we are in the normal mode of Vim.
  
100k and 100h are used to move cursor to top-left. 
  
Then use 11j 75l and 4l to locate to the bug in the code where the two lists being merged are in the wrong order. 
  
Use r2 and r1 to change 2 to 1 and 1 to 2.

Then press :wq and enter to save and quit.
```
vim L Tab .j <Tab> <enter>
```
By pressing Tab, it is autocomplete with vim ListExamples.java

Now editing the file ListExamples.java.
```
<esc> 100k 100h 42j 11l r2 :wq <enter>
```
Pressing esc allows us to make sure we are in the normal mode of Vim.
  
100k and 100h are used to move cursor to top-left.

Use 42j and 11l to locate to the bug in the code where the index being added should be index 2 instead of index 1 in the final loop.

Use r2 to replace the 1 with 2.

Then press :wq and enter to save and quit.

<img width="1023" alt="截屏2023-05-17 19 33 23" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/83fdc36b-b9cc-49fc-804c-57ac748322a0">
<img width="711" alt="截屏2023-05-17 19 33 40" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/ca96da23-fbf1-4153-ad65-a40aa8ef928c">

# Step 8: Run the tests, demonstrating that they now succeed
```
Keys pressed: <up><up><up><enter>
```
Run bash test.sh. This command is 3 up in history.

<img width="401" alt="截屏2023-05-17 19 34 06" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/7d4fefac-050d-4f10-a4c2-db9ebf0baedc">

# Step 9: Commit and push the resulting change to your Github account
```
$ git commit --amend
<enter>
$ git push origin main
<enter>
```
<img width="597" alt="截屏2023-05-17 19 41 09" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/10cfbbc1-912b-450a-8b09-fff0bfa60266">
<img width="522" alt="截屏2023-05-17 20 00 22" src="https://github.com/kevinnie2003/cse15l_lab4/assets/122497019/299c01e4-b52e-4fba-88dc-e48ce602b0d0">
