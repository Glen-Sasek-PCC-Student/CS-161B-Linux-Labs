# Linux Lab 3 \- Advanced Vim commands

## Instructions for Lab 3

1. Watch the videos in Module 9, Lesson **Linux Tutorials** before you do this Lab 3\. You must have completed the practice in Chapters 3.3 and 3.4 in the [PCC Linux and Vim Manual](https://docs.google.com/document/d/1Ap4xFkNUkUbi7kYteg0KEIu9I9_hAuDZBtubA3ExxLM/edit?usp=sharing) to be able to do this lab.  
2. Here is a [Video for Lab3](https://youtu.be/3CAcTuoTMfM), that you can follow along as you do this Lab.  
3. First, login to PCC Linux Server (**cslinux.pcc.edu**)  
4. Make sure you are in your home directory.  
5. (Your home directory should look like this: **yourname@vmcslinuxprod01:\~/**)  
6. If not type **cd** and hit enter to get you back to the home directory  
7. From your home directory, start the **script** command \- type **script lab3.txt** at the command line.  
8. List the files in your current directory	**ls**  
9. Move into the directory for your class 	**cd  CS161B**  
10. Make a new directory for Lab3 	**mkdir Lab3**  
11. Change into that directory    	**cd Lab3**  
12. Copy a file from my folder to your folder 

    **cp \~gd.iyer/CS161B/samples/sample\_a06.cpp .** 

    (Do not forget the period at the end, this tells the command to copy the file to your current folder.) 

13. Copy another file from my folder to your folder 

    **cp \~gd.iyer/CS161B/samples/items.txt .** 

14. (Do not forget the period at the end, this tells the command to copy the file to your current folder.)  
15. Type **vi sample\_a06.cpp** and hit enter  
16. Search for a word by typing	**/main**  
17. Delete the word you searched for by typing **dw**  
18. **T**ype **u** to undo the last delete  
19. Go to line 21 \- type **:21** (You should be on the calcCalories function prototype line)  
20. To replace all occurrences of the word **size** in the current line type:  
                            **:s/size/count/g**

21.  To search and replace the word in the entire file, use the percentage character % as a range.			**:%s/size/count/g**  
22. Go to line 21 \- type **:21** (You should be on the calcCalories function prototype line)  
23. Type **yy** to yank that line.  
24. Type **GG** to go to the end of the file.  
25. Type **p** to paste the line you copied in step 21\.  
26. Type **:89** to go to line 89\.  
27. Type **13yy** to yank or copy 13 lines.  
28. Type **GG** to go to the end of the file and type **p** to paste them.  
29. Type **:102** to go to line 102\.  
30. Type **15dd** to delete all the lines we pasted.  
31. When you are done, hit the escape key  
32. Now you can quit saving your changes	**:wq**  
33. The next step is to compile the C++ source code file. To compile the sample\_a06.cpp code type:  
    **g++ \-Wall \-g sample\_a06.cpp \-o sample\_a06**  
34. If there are syntax errors, examine the line number of the first 2 or 3 errors and fix those before continuing. To fix the syntax errors use the Linux editor again:  
    **vi sample\_a06.cpp**  
35. To run your program type **./sample\_a06**, and the output will appear directly below.   
36. Type **exit** and you are almost done with Lab 3 and you should have a **lab3.txt** file.  
37. Type **ls** to list the contents of your directory. You should see **lab3.txt**  
38. Follow the instructions in the Transferring Files section of your PCC Linux Manual and transfer the file to your pc and upload to D2L with assignment 7\.  
39. Now you are done with Lab 3\.