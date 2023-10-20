# Lab Report 1 
## Henry Huynh | CSE 15L
    [user@sahara ~]$ cd
    [user@sahara ~]$ cd lecture1
    [user@sahara ~/lecture1]$ cd messages
    [user@sahara ~/lecture1/messages]$ cd en-us.txt
    bash: cd: en-us.txt: Not a directory
The working directory when each command was ran was in this order,
<br> 
1) \home  
2) \home  
3) \home\lecture1\
4) \home\lecture1\messages  
   
In the case of the cd command, it does not directly return anything in the next line but rather, another prompt is returned again with the updated directory.  
In the case of **cd** in the first line, since we did not specify any directory to move into the next prompt retured what it was before which was [user@sahara ~]$ 
The command can take no argument and works as intended.  
Looking at the second input lined we changed directory into lecture1 which is represented in the 3rd prompt with [user@sahara ~/lecture1]$
Again this is behaving as expected since it is changing our directory into the lecture1 folder.
Just like the 2nd prompt, in the 3rd line I wanted to move into the messages folder and behaves as expected, which is reflected in the 4th prompt. 
Which prints [user@sahara ~/lecture1/messages]$ showing us we have moved into the folder.
Lastly trying to move into a file using **cd** into a text file, we get an error which reads "bash: cd: en-us.txt: Not a directory".
Even if it returns an error, **cd** is behaving as expected because we cannot change directories into a file. 

![image](https://github.com/huynhhenry/cse15l-lab-reports/assets/146884910/d79b2cb3-fe62-4e52-b5e6-de6ec027058f)
The working directory when as command was ran was in this order,
1) \home  
2) \home  
3) \home  

I got this output because that is how the file structure is when cloning te lab, and ls does not
change the working directory leaving it to stay at the base state.
The output is correct and **ls** is behaving as expected because when including files at the end of a tree it appends it onto the end.  
The terminal returns the directories and files in the next line after using a **ls** command and in EdStems case, directories were highlighted with blue.   

![image](https://github.com/huynhhenry/cse15l-lab-reports/assets/146884910/c1835478-75c1-4a94-92f2-999d5590e6bc)
For the **cat** command the working directory for all three lines is,
1) \home  
2) \home  
3) \home  

**cat** does not change the working directory either only **cd** does leaving it to be the same. The first line with
just cat ended in an error because it has nothing to read, I used *ctrl + c* to kill the command or *ctrl + d* to start
a new line. The second line gave a missue line saying it is a directory which makes sense becasue it should be used on files 
to concatenate the text inside. The 3rd line performed as expected and printed "Hello World!"
