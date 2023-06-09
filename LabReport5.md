# Lab Report 5: Debugging

## Student Post
**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

System information: (Mac M1 (ARM), MacOS: 13.3.1 (22E261), safari, vscode)

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

Currently I have created an implementation for merge sort however when I run merge sort on a given array, It sorts it but does not have all the correct elements, it seems like it just removes a bunch. Screenshots will be provided below:
![Server Running 1](LBR5-1.png)

**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

The command I am running is:
```
$ bash run.sh
```
Run.sh contains:
```
javac *.java
java Main
```
The main file contains:
```
int[] arr = {1, 22, 14, 2, 3, 6, 4, 10, 11, 4};
MergeSort.mergeSort(arr);
System.out.println(Arrays.toString(MergeSort.mergeSort(arr)));
```
## TA Response
Thank you for the in depth response. According to the information provided it seems that the bug is most likely in the MergeSort class. It also seems like there is a minor issue when iterating through the arrays. So take a closer look when going through and specifically check the variables. If this response is not enough you can follow up or go to office hours.

## Student Second Attempt
Thank you so much for your advice, you were correct in the index part. I accidentally updated the wrong variable in one of the loops. So line 63 should have `i2++;` instead of `i1++;`. Really the error just resulted in the right side adding the same variable over and over. Below is a screenshot of the fixed code and proper output.
![Server Running 1](LBR5-2.png)

## Recap
1) The file and directory structure is not relevant
2) Contents:
Before:
![Server Running 1](LBR5-1.png)
After:
![Server Running 1](LBR5-2.png)
3) Command Line
```
javac *.java
java Main
```
4) To fix the bug in the end I simply changed what value was updated on line 63.

## Reflection
In a couple of sentences, describe something you learned from your lab experience in the second half of this quarter that you didn’t know before. It could be a technical topic we addressed specifically, something cool you found out on your own building on labs, something you learned from a tutor or classmate, and so on. It doesn’t have to be specifically related to a lab writeup, we just want to hear about cool things you learned!
I really enjoyed learning vim because it showed me how to to use just to command line to be able to clone a file from online, edit it, and then push it back to github all while staying in the command line. Overall this class taught me so much about servers and how to run them remotely (now  I know how to make a minecraft server on a remote server)
