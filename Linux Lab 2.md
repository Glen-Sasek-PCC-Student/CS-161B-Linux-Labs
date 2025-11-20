# Linux Lab 2 \- Basic Vim commands

## Instructions for Lab 2

1. Watch the videos in Module 7, Lesson **Linux Tutorials** before you do this Lab 2\. You must have completed the practice in Chapters 3.1 and 3.2 in the [PCC Linux and Vim Manual](https://docs.google.com/document/d/1Ap4xFkNUkUbi7kYteg0KEIu9I9_hAuDZBtubA3ExxLM/edit?usp=sharing) to be able to do this lab.  
2. Here is a [Video for Lab2](https://youtu.be/o37NNh5Ml5I), that you can follow along as you do this Lab.  
3. First, login to PCC Linux Server (**cslinux.pcc.edu**)  
4. Make sure you are in your home directory.  
5. (Your home directory should look like this: **yourname@vmcslinuxprod01:\~/**)  
6. If not type **cd** and hit enter to get you back to the home directory  
7. From your home directory, start the **script** command \- type **script lab2.txt** at the command line.  
8. List the files in your current directory	**ls**  
9. Move into the directory for your class 	**cd  CS161B**  
10. Make a new directory for Lab2 	**mkdir Lab2**  
11. Change into that directory    	**cd Lab2**  
12. Copy a file from my folder to your folder 

    **cp \~gd.iyer/CS161B/samples/sample\_a01.cpp .** 

    (Do not forget the period at the end, this tells the command to copy the file to your current folder.) 

13. Type **vi sample\_a01.cpp** and hit enter  
14. Insert header comments to your file by typing **i** followed by comments  
15. Now type uppercase  **ZZ \-** Did your changes get saved?   
16. Reopen your file, type **vi sample\_a01.cpp** and hit enter  
17. Let’s try going to the end of your file, type	**G**  
18. Now go back to the beginning of the file, type	 **gg**  
19. Page down by holding down **control** key and hit **d	CTRL+d**  
20. Page up by holding down the **control** key and hit **b	CTRL+b**  
21. Go to a specific line in the document (e.g., line 50\)	**:20**  
22.  Go to the end of the line, type			**$**  
23. Type some random text \- remember to go to insert mode.  
24. When you are done, hit the escape key  
25. Now you can quit without storing your changes	**:q\!**  
26. The next step is to compile the C++ source code file. To compile the sample\_a01.cpp code type:  
    **g++ \-Wall \-g sample\_a01.cpp \-o sample\_a01**  
27. If there are syntax errors, examine the line number of the first 2 or 3 errors and fix those before continuing. To fix the syntax errors use the Linux editor again:  
    **vi sample\_a01.cpp**  
28. To run your program type **./sample\_a01**, and the output will appear directly below. Test your program several times with different inputs and make sure your code is working properly.  
29. Type **exit** and you are almost done with Lab 2 and you should have a **lab2.txt** file.  
30. Type **ls** to list the contents of your directory. You should see **lab2.txt**  
31. Follow the instructions in the Transferring Files section of your PCC Linux Manual and transfer the file to your pc and upload to D2L with assignment 6\.  
32. Now you are done with Lab 2\.