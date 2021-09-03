# ME 701 -- Homework 1 -- Ezekial Jimenez

## Instructions

Your solution should be an update to this `README.md` file that will be
committed back to your repository created when you clicked the HW 1 link.

## Problem 1 -- Open-Source Software

### Statement

Think of the things you do routinely on a computer that require
specific software packages.  Find an
open-source solution from the software repository
for one of these activities and tell me about it in 100 words or less.
For example, I used to do lots of audio recording when I was in
high school (not *that* long ago) and used special (and
pretty expensive) tools like
Cakewalk Sonar.  Since then, I've found an
open-source package for doing multitrack
recording called Ardour that doesn't have all the bells and
whistles but, because I can program in C++ and the
source code is available, I could, in theory,
create any such whistles I need.  **Note**: You may not
describe anything already discussed in class (e.g., the LibreOffice suite
or Octave).

### Solution

I have used 3D modeling software like SolidWorks or CAD to come up with designs for 3D printing. 
There is an open-source software called Blender that is used similarly. It began development in 1994
and has been updated and maintained since then by a community of developers.

## Problem 3 -- Your CPU

### Statement

Figure out how to display information about your CPU via the
command line.  This should include at least the **processor
speed** and the **number of cores**.  Describe your command(s) below.
(Hint: redirection is helpful; remember, that's like
using `ls > directory_contents.txt` to dump the contents of a directory to a file.

### Solution

To display CPU information, I used the following command:

```bash
cat /proc/cpuinfo
```
The processor speed is shown at the end of the model name field, and 
the number of cores is shown after the cpu cores field.
## Problem 4 -- Resource Hogs

### Statement

Figure out how to list the programs that use the most
amount of (1) processing and (2) memory.  Describe your command(s)
in your writeup.

### Solution

To show the list of top memory and processing users, I endered the following command:

```bash
ps -eo pid,ppid,cmd,%mem,%cpu --sort=-%mem | head
```
I found this at the following website: https://www.tecmint.com/find-linux-processes-memory-ram-cpu-usage/
The command shows the highest usage programs in descending order.

## Problem 5 -- `bash`

### Statement

Where is `bash` located on your Linux system?  And what version of
`bash` are you using?  Make sure to provide any commands you use to
determine this information.

### Solution

`bash` is in the location /usr/bin/bash 
I found this by typing: 
```bash
which bash
```
I am using version 5.0.17(1) of `bash`
I found this by typing the following command:
```bash
bash --version
```
