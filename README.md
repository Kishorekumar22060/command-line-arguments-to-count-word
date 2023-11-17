# Ex5b-command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import sys module to use command line arguments
### Step 2: 
Use the open() by getting the file name with "sys.argv[1]" which means the first index of given argument
### Step 3: 
Iterate the content of the file using for loop.
### Step 4:  
Split the contents into each line using .split() function.
### Step 5: 
Iterate the list of lines and increment the value of variable (word) each time.
### Step 6: 
Run the program by giving "python prgm.py EX12.txt" on the terminal.
## PROGRAM:
```
#Developed By: KISHORE KUMAR U
#Register No: 212222233003
import sys
fp=open(sys.argv[1],"r")
d={}
for i in fp:
    for w in i.split():
        if w not in d.keys():
             d[w]=1
        else:
            d[w]+=1
print(d)       
```
### OUTPUT:
![282657615-7f0437f1-17c7-489d-b02b-d2fdd2061947](https://github.com/Kishorekumar22060/command-line-arguments-to-count-word/assets/141472136/6717650c-35a1-4392-8ccd-6d67c7cb1d4e)



## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
