# Linux Lab 3 \- Advanced Vim commands

## Instructions for Lab 3

Read Chapters 3.3 and 3.4 in the [PCC Linux and Vim Manual](https://docs.google.com/document/d/1Ap4xFkNUkUbi7kYteg0KEIu9I9_hAuDZBtubA3ExxLM/edit?usp=sharing) to prepare for this lab.  
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
5. Make a new directory for Lab3.  
   ```mkdir Lab3```  
6. Change into that directory  
   ```cd Lab3``` 
7.  Copy a file from a different folder to your folder.  
   ```cp ~gd.iyer/CS161B/samples/sample_a06.cpp .```  
   **Include the period at the end, this tells the command to copy the file to your current folder.** 
8. Copy another file to your folder.  
   ```cp ~gd.iyer/CS161B/samples/items.txt .```   
   **Include the period**  
9. Open the file in the vim editor.  
   ```vim sample_a06.cpp``` 
10. Search for the word "main" by typing **/main**  
11. Delete the word you searched for by typing **dw**  
12. Type **u** to undo the last delete  
13. Go to line 21, type **:21** (You should be on the calcCalories function prototype line)  
14. To replace all occurrences of the word **size** with **count** in the current line type:  **:s/size/count/g**
15.  To search and replace the word in the entire file, use the percentage character % as a range. **:%s/size/count/g**  
16. Go to line 21, type **:21** (You should be on the calcCalories function prototype line)  
17. Type **yy** to yank that line. yank is like copy  
18. Type **GG** to go to the end of the file.  
19. Type **p** to paste the line you copied in step 21.  
20. Type **:89** to go to line 89.  
21. Type **13yy** to yank or copy 13 lines.  
22. Type **GG** to go to the end of the file and type **p** to paste them.  
23. Type **:102** to go to line 102.  
24. Type **15dd** to delete all the lines we pasted.  
25. Enter command mode by pressing **esc**  
26. Write and quit **:wq**  
27. The next step is to compile the C++ source code file.   
    ```g++ -Wall -g sample_a06.cpp -o sample_a06```
28. If there are syntax errors, examine the line number of the first 2 or 3 errors and fix those before continuing. To fix the syntax errors use the Linux editor again:   
    ```vim sample_a06.cpp```  
    Or, press the up arrow to re-use a previous command.  
29. Run your program.  
    ```./sample_a06```
30. Save your command history in a file named **lab3.txt**  
    ```history > lab3.txt```  
31. Verify the file was created.  
    ```ls```  
    You should see **lab3.txt**   
    Optional: view the file content.  
    ```cat lab3.txt``` 
32. Download the file from our Linux server to your local machine.
33. Upload to D2L. 