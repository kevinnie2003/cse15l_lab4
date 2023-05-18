# Step 4: Log into ieng6
```
$ ssh cs15lsp23cx@ieng6.ucsd.edu
<enter>
```
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
```
Keys pressed: vim L <Tab> T <Tab> <enter>
# Now editing the file ListExamplesTest.java.
<esc> 100k 100h 11j 75l r2 4l r1 :wq <enter>
# Move cursor to top-left. Locate to the bug in the code where the two lists being merged are in the wrong order. Change 2 to 1 and 1 to 2.
vim L Tab .j <Tab> <enter>
# Now editing the file ListExamples.java.
<esc> 100k 100h 42j 11l r2 :wq <enter>
# Move cursor to top-left. Locate to the bug in the code where the index being added should be index 2 instead of index 1 in the final loop.

```

# Step 8: Run the tests, demonstrating that they now succeed
```
Keys pressed: <up><up><up><enter>
# run bash test.sh. This command is 3 up in history.
```
