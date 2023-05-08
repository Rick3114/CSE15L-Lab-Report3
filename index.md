# LabReport3

## Different Ways to Use `grep` Command: 
`grep` is an important command that allows us search for text patterns within a file. It is useful for searching for specific words or letters within a givin file. The `grep` command has over 40 different options that each do differnet things here are examples of some. 

**Command1: Firt Word In Line**  
``$ grep "^(insert word of choice of here)" (insert file being searched here)``
This command returns all the lines in the given file that start with the word that was being searched for.
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
The example above is used in the directory of Alchol_Problems on the file Session2-PDF.txt. The command searches through the file and returns all the lines within the file that start with the word "Many".

**Why Useful:**\
This command can come in handy when you recall the first word of a specific line, but forgot where it is located, the command will call up all the lines that start with your given word and you will be able to more quickly fine the line and information you need.\

**Source:**\
[https://www.softwaretestinghelp.com/grep-command-in-unix/](https://www.softwaretestinghelp.com/grep-command-in-unix/)

**Command2: Last Word In Line**\
``$ grep "(insert word of choice here$)" (insert file of choice here)``\
This command returns all the lines in the file that end with the given word.\
**Example1:** 

**Input:** 
```
$ grep "emergency$" Session3-PDF.txt 
```
**Output:** 
```
among the patients who are triaged and treated in emergency
settings.4,7 The prevalence of this co-factor to the emergency
intervening effectively with alcohol problems in emergency
patients with alcohol problems encountered in the emergency
among participants in control conditions. After the emergency
which lasted 30 to 40 minutes, was delivered in the emergency
To some degree, all interventions described in the emergency
Issues and challenges for interventions in emergency
interventions have been able to get a number of emergency
low BAC testing rates for intoxicated drivers by emergency
long-term outcomes should be introduced into several emergency
direction as to how to implement interventions in emergency
and uniformly applied to every patient admitted to the emergency
2. Degutis LC. Screening for alcohol problems in emergency
injuries, and dangerous behaviors-and the revolving emergency
hospital emergency
alcohol health worker in an accident and emergency
1. D'Onofrio G, Degutis LC. Preventative care in the emergency
New directions in brief alcohol interventions in emergency
alcohol health worker in an accident and emergency
both a unique opportunity for an intervention in the emergency
need to be figuring out how to connect primary care and emergency
```
The example above is used in the directory of Alchol_Problems on the file Session3-PDF.txt. The command searches through the file and returns all the lines within the file that end with the word "emergency". 

**Example2:**

**Input:**




