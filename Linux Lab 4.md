# Linux Lab 4 \- gdb

## Instructions for Lab 4

Read Chapter 5 in the [PCC Linux and Vim Manual](https://docs.google.com/document/d/1Ap4xFkNUkUbi7kYteg0KEIu9I9_hAuDZBtubA3ExxLM/edit?usp=sharing) to prepare for this lab.  

1. login to PCC Linux Server (**cslinux.pcc.edu**).  
   ```ssh your.name@cslinux.pcc.edu``` 
2. Check you are working in your home directory.  
   ```cd```  
   The cd command with no additional parameters changes to your home directory.
   (Your home directory should look like this: **yourname@vmcslinuxprod01:\~/**)  
   ```pwd```  
   Print the working directory.  
3. List the files in your current directory.    
   ```ls```
4. Move into the directory for your class.  
   ```cd  CS161B```  
   If this directory does not exist, make it, then cd to it.  
   ```mkdir CS161B```   
   ```cd CS161B```
5. Make a new directory for Lab4.  
   ```mkdir Lab4```  
6. Change into that directory  
   ```cd Lab4``` 
7.  Copy a file from a different folder to your folder.  
   ```cp ~gd.iyer/CS161B/samples/debug/nestedBug.cpp .```  
   **Include the period at the end, this tells the command to copy the file to your current folder.** 
8. Open the file in the vim editor.  
   ```vim nestedBug.cpp```  
9.  Notice the code has a nested loop and is trying to print a tic tac board like this:   
    ```
    X    O    X    
    O    X    O    
    X    O    X
    ```
10. Compile the file.  
    ```g++ -Wall -g nestedBug.cpp -o nestedBug```
11. Run the program. 
    ```./nestedBug```  
    Notice the output is not what you expected, even though we did not get any compile errors.  
12. Run your code using the debug program **gdb**.  
    ```gdb ./nestedBug```    
    You should have a **(gdb)** prompt.  
    gdb has good built in help if you need it.
13. Type **b 12** to set a breakpoint on line 12.  
14. Now type **r** to run your program.  
15. Your program should run to line 12 and wait. Type **n** to execute the next line.  
16. You should see the output line on the screen.  
17. Type **n** again to execute the next line. Now you are going through the for loop.  
18. Type **p i** to print the value of **i**. You can watch your variables using the **p** command and you can step through your code using **n**.  
19. See if the variables **i** and **j** are doing what you expect them to do as you step through the code. Watch the Linux Lab 4 Video to see how I do this if you are not sure.  
20. When you find the bug, fix the code file. 
21. Re-compile the file and run the program.  
    ```g++ -Wall -g nestedBug.cpp -o nestedBug```     
    ```./nestedBug```    
22. Verify you fixed the bug.  
23. Save your command history in a file named **lab4.txt**  
    ```history > lab4.txt```  
31. Verify the file was created.  
    ```ls```  
    You should see **lab4.txt**   
    Optional: view the file content.  
    ```cat lab4.txt``` 
32. Download the file from our Linux server to your local machine.
33. Upload to D2L. 