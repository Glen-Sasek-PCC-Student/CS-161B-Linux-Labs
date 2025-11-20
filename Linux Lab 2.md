# Linux Lab 2 \- Basic Vim commands

## Instructions for Lab 2

Read Chapters 3.1 and 3.2 in the [PCC Linux and Vim Manual](https://docs.google.com/document/d/1Ap4xFkNUkUbi7kYteg0KEIu9I9_hAuDZBtubA3ExxLM/edit?usp=sharing) to prepare for this lab.  

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
5. Make a new directory for Lab2.  
   ```mkdir Lab2```  
6. Change into that directory  
   ```cd Lab2```  
7. Copy a file from my folder to your folder.  
   ```cp ~gd.iyer/CS161B/samples/sample_a01.cpp .```  
   (Include the period at the end, this tells the command to copy the file to your current folder.) 
8. Open the file in the vim editor.  
   ```vim sample_a01.cpp```   
9. Insert header comments with your name and date.  
   The vim editor opens in command mode.   
   **Press i to enter Insert mode, then add comments**.  
   ```
   // Your Name  
   // Todays Date
   ```  
10. Now type **esc** to enter command mode then uppercase **ZZ** to save and quit.  
    Recall from Lab 1 we can also save and quit with the sequence **esc:wq**    
11. Reopen your file.  
    ```vim sample_a01.cpp```   
    Or, press the up arrow to re-use a previous command.  
12. Go to the end of your file, type **G**   
    Instructions 12 through 17 must be done in command mode.  
    Enter command mode by pressing **esc**  
    You can always press **esc** if you are not sure of your current mode. 
13. Go to the beginning of the file, type **gg**  
14. Page down by holding down **control** key and hit **d CTRL+d**  
15. Page up by holding down the **control** key and hit **b	CTRL+b**  
16. Go to a specific line in the document e.g., line 20 press colon : followed by the number **:20**  
17. Go to the end of the current line, type	**$**  
18. Use the **i** command to enter insert mode and add some random characters.  
19. Enter command mode by pressing **esc**  
20. Now you can quit without storing your changes **:q!**  
21. The next step is to compile the C++ source code file. To compile the sample_a01.cpp code type:  
    ```g++ -Wall -g sample_a01.cpp -o sample_a01```  
22. If there are syntax errors, examine the line number of the first 2 or 3 errors and fix those before continuing. To fix the syntax errors use the Linux editor again:    
    ```vim sample_a01.cpp```   
    Or, press the up arrow to re-use a previous command.  
23. Run your program.  
    ```./sample_a01```   
    Test your program several times with different inputs.
24. Save your command history in a file named **lab2.txt**  
    ```history > lab2.txt```  
25. Verify the file was created.  
    ```ls```  
    You should see **lab2.txt**
    Optional: view the file content.  
    ```cat lab2.txt``` 
26. Download the file from our Linux server to your local machine.
27. Upload to D2L. 