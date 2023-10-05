# Lab Report 1 
## Henry Huynh | CSE 15L
    [user@sahara ~]$ cd
    [user@sahara ~]$ cd lecture1
    [user@sahara ~/lecture1]$ cd messages
    [user@sahara ~/lecture1/messages] cd en-us.txt
    bash: cd: en-us.txt: Not a directory
The working directory when each command was ran was in this order,
1) /home
2) /home
3) /home/lecture1
4) /home/lecture1/messages
   
The next line after changing directories gave us the result of my command, showing where I was
in the directory. In this case the **cd** command worked as intended until trying to change directories 
into a file resulting in an error. **cd** only works with directories and not files.

![image](https://github.com/huynhhenry/cse15l-lab-reports/assets/146884910/d79b2cb3-fe62-4e52-b5e6-de6ec027058f)
The working directory when as command was ran was in this order,
1) /home
2) /home
3) /home

I got this output because that is how the file structure is when cloning te lab, and ls does not
change the working directory leaving it to stay at the base state. The output is correct and **ls** is behaving 
as expected because when including files at the end of a tree it appends it onto the end.

![image](https://github.com/huynhhenry/cse15l-lab-reports/assets/146884910/c1835478-75c1-4a94-92f2-999d5590e6bc)
For the **cat** command the working directory for all three lines is,
1) /home
2) /home
3) /home

**cat** does not change the working directory either only **cd** does leaving it to be the same. The first line with
just cat ended in an error because it has nothing to read, I used *ctrl + c* to kill the command or *ctrl + d* to start
a new line. The second line gave a missue line saying it is a directory which makes sense becasue it should be used on files 
to concatenate the text inside. The 3rd line performed as expected and printed "Hello World!"
