# Linux Lab 1 \- Using the Command Line

## Instructions for Lab 1

Watch the videos in Module 6, Lesson **Linux Tutorials** before you do this Lab 1\. Read Chapters 1 and 2 in the [PCC Linux and Vim Manual](https://docs.google.com/document/d/1Ap4xFkNUkUbi7kYteg0KEIu9I9_hAuDZBtubA3ExxLM/edit?usp=sharing) to prepare for this lab. 


1. login to PCC Linux Server (**cslinux.pcc.edu**).  
   ```ssh your.name@cslinux.pcc.edu``` 
2. Make sure you are in your home directory.  
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
5. Make a new directory for Lab1.  
   ```mkdir Lab1```  
6. Change into that directory  
   ```cd Lab1```  
7. Create a file named lab1.cpp using the vim editor.  
   ```vim lab1.cpp```
8. Insert header comments with your name and date.  
   The vim editor opens in command mode.   
   **Press i to enter Insert mode, then add comments**.  
   ```
   // Your Name  
   // Todays Date
   ```    
9.  Press the escape **esc** key to return to command mode.
10. Press the colon **:** key to enter last line mode.  
11. Save your work by typing **w** followed by enter. This is the write command.  
12. Add hello world code to this cpp file.  
    ```
    #include <iostream>

    using namespace std;

    int main() {
        cout << "Hello, World!" << endl;
    }
    ```
13. Press the escape **esc** key to return to command mode. 
14. Press the colon **:** key to enter last line mode.
15. Save and quit your work by typing **wq** followed by enter. You can combine w and q to write and quit or use each alone.  
16. The next step is to compile the C++ source code file. To compile the lab1.cpp code type:  
    ```g++ -Wall -g lab1.cpp -o lab1```  
17. If there are syntax errors, examine the line number of the first 2 or 3 errors and fix those before continuing. To fix the syntax errors use the Linux editor again:    
    ```vim lab1.cpp```  
18. Run your program.  
    ```./lab1```
19. Save your command history in a file named **lab1.txt**  
    ```history > lab1.txt```  
20. Verify the file was created.  
    ```ls```  
    You should see **lab1.txt**
    Optional: view the file content.  
    ```cat lab1.txt``` 
21. Download the file from our Linux server to your local machine.
22. Upload to D2L.  
    
For help downloading and uploading to D2L see the instructions in the Transferring Files section of your PCC Linux Manual.
