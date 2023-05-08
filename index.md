# LabReport3

## Different Ways to Use `grep` Command: 
`grep` is an important command that allows us search for text patterns within a file. It is useful for searching for specific words or letters within a givin file. The `grep` command has over 40 different options that each do differnet things here are examples of some. 

**Command1: Firt Word In Line**  
``grep "^(insert word of choice of here)" (insert file being searched here)``
This command returns all the lines in the given file that start with the word that was being searched for.\
**Example1:**

**Input:** 
``` 
$ grep "^The" chapter-1.txt
```
**Output:** 
``` 
The FAA and NORAD
The Agencies Confer
The Pentagon Teleconferences. Inside the National Military Command Center, the deputy director for operations immediately thought the second strike was a terrorist attack. The job of the NMCC in such an emergency is to gather the relevant parties and establish the chain of command between the National Command Authority-the president and the secretary of defense- and those who need to carry out their orders.
```
The example above is used in the directory of 911report on the file chapter-1.txt. The command searches through the file and returns all the lines within the file that start with the word "The". 

**Example2:** 

**Input:** 
```
$ grep "^Many" Session2-PDF.txt
```
**Output:** 
```
Many patients in the emergency department (ED) have alcohol
Many injured ED patients are screened with a BAC, which can help
```
The example above is used in the directory of government on the file Session2-PDF.txt. The command searches through the file and returns all the lines within the file that start with the word "Many".
**Why Useful:** 
This command can come in handy when you recall the first word of a specific line, but forgot where it is located, the command will call up all the lines that start with your given word and you will be able to more quickly fine the line and information you need.\
**Source:**\
[https://www.softwaretestinghelp.com/grep-command-in-unix/](https://www.softwaretestinghelp.com/grep-command-in-unix/)


