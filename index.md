# LabReport3

## Different Ways to Use `grep` Command: 
`grep` is an important command that allows us to search for text patterns within a file. It is useful for searching for specific words or letters within a givin file. The `grep` command has over 40 different options that each do differnet things here are examples of some. 

## Command1: Firt Word In Line 
``$ grep "^(insert word of choice of here)" (insert file being searched here)``\
This command returns all the lines in the given file that start with the word that was being searched for.

### Example1:

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

### Example2:

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
This command can come in handy when you recall the first word of a specific line, but forgot where it is located. The command will call up all the lines that start with your given word and you will be able to find the line and information you need faster rather than personally searching each individual line.

**Source:**\
[https://www.softwaretestinghelp.com/grep-command-in-unix/](https://www.softwaretestinghelp.com/grep-command-in-unix/)

## Command2: Last Word In Line
``$ grep "(insert word of choice here$)" (insert file being searched here)``\
This command returns all the lines in the file that end with the given word.

### Example1: 

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

### Example2:

**Input:**
```
$ grep "legal$" 5_Legal_Groups.txt
```
**Output:**
```
Five independent Salt Lake organizations that provide legal
campaign by an alliance of the non-profit providers of free legal
```
The example above is used in the directory of Media on the file 5_Legal_Groups.txt. The command searches through the files and returns all the lines within the file that end with the word "legal".

**Why Useful:**\
This command can come in useful when you want to see how many times you ended a sentence a certain way. Or when see how a certain sentece ends and the context that lead up to the ending of that sentence. 

**Source:**\
[https://www.softwaretestinghelp.com/grep-command-in-unix/](https://www.softwaretestinghelp.com/grep-command-in-unix/)

## Command3: Finding Specific Word:
``$ grep -i "(insert word of choice here)" (insert file being searched here)``\
This command returns all the lines within the file that contain the word that is being searched for in either lower-case or uppercase it does not matter.

### Example1: 

**Input:**
```
$ grep -i "clean" bill.txt
```
**Output:**
```
To amend the Clean Air Act to reduce air pollution through
"Sec. 408. Clean coal technology regulatory incentives. "Sec. 409.
Title IV of the Clean Air Act (relating to acid deposition
SEC. 408. CLEAN COAL TECHNOLOGY REGULATORY INCENTIVES.
Definition.- For purposes of this section, "clean coal
Revised Regulations for Clean Coal Technology
permanent clean coal technology demonstration project. For the
purposes of this section, a clean coal technology demonstration
heading "Department of Energy- Clean Coal Technology", up to a
clean coal technology, or similar projects
or removal of a temporary cleancoal technology demonstration
Permanent projects.- For permanent clean coal technology
Exemption for Reactivation of Very Clean Units.- Physical
enactment of the Clean Air Act Amend- meats of 1990);
coal-fired boiler with one of thefollowing clean coal technologies:
oil-and gas-fired unit which has beenawarded a clean coal
titles of the Clean Air Act with respect to:
(a) Title I of the Clean Air Act is amended by-
Title III of the Clean Air Act is amended by modifying
Title IV of the Clean Air Act (relating to noise
Title VIII of the Clean Air Act Amendments of 1990
title IV of the Clean Air Act shall also monitor carbon dioxide
Clean Air Act shall apply for purposes of this section in the same
```
The example above is used in the directory of Env_Prot_Agen on the file bill.txt. The command searches through the file and returns all the lines within the file that contain the word "clean". 

### Example2: 

**Input:** 
```
$ grep -i "vitamin" journal.pbio.0020012.txt
```
**Output:**
```
designer chocolate with a clear conscience. The demographer sticks to vitamin supplements,
all, as well as taking vitamin supplements.
```
The example above is used in the directory of plos on the file journal.pbio.0020012.txt. The command searches through the file and returns the lines within the file that contain the word "vitamin". 

**Why Useful:**\
This command can come in useful when you want to search for a specific theme or topic, you serach using a key word and find the lines that correlate with it. 

**Source:**\
[https://www.softwaretestinghelp.com/grep-command-in-unix/](https://www.softwaretestinghelp.com/grep-command-in-unix/)

## Command4: Count Of Specific Word
``$ grep -c "(insert word of choice here)" (insert file that is being searched) ``\
This command returns the count of the number of times the given word appears in the given file. 

### Example1: 

**Input:** 
```
$ grep -c "postal" Cohenetal_comparison.txt
```
**Output:** 
```
35
```
The example above is used in the directory of Post_Rate_Comm on the file Cohenetal_comparison.txt. The command searches through the file and counts the amount of times the word "postal" appears in the file and returns the total count which is 35.

###  Example2:

**Input:**
```
$ grep -c "cells" 1471-213X-1-11.txt 
```
**Output:**
```
113
```
The example above is used in the directory of biomed on the file 1471-213X-1-11.txt. The command searches through the file and counts the amount of times the word "cells" appears in the file and returns the total count which is 113.

**Why Useful:**\
This command could be useful when looking at data and wanting to see how much a certain variable is shown. Or when looking at a file, depending whether you use a key word to searh for a certain topic, it shows how much that word appears in the file giving somewhat of an idea of how influential and imporant that topic is in the file. 

**Source:**\
[https://www.youtube.com/watch?v=EQLFr8uC44k](https://www.youtube.com/watch?v=EQLFr8uC44k)









