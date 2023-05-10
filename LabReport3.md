# Lab Report 3
The command that will be used in this report will be the `grep` command
## Option 1: -i
This command can be used like:
```
$ grep "hello" -i technical/911report/*.txt
technical/911report/chapter-1.txt:    At 10:39, the Vice President updated the Secretary on the air threat conference: Vice President: There's been at least three instances here where we've had reports of aircraft approaching Washington-a couple were confirmed hijack. And, pursuant to the President's instructions I gave authorization for them to be taken out. Hello?
```
In this example the command being used was -i which stands for ignore case. So in this instance grep searched through all the text files in technical/911report and checked if they contained the word `hello` (regardless of the case). Then it printed out the linked in which it was found. This is a good example becuase it demonstrates the ignoring case, becuase the word found was `Hello` with a capital H, therefore revealing the case was ignored.
Another example would be:
```
[cs15lsp23pg@ieng6-203]:stringsearch-data:201$ grep "BANANA" -i technical/biomed/*.txt
technical/biomed/1471-2105-3-6.txt:          fond of bananas." and "I am of very fond bananas. Am I a
technical/biomed/1471-2105-3-6.txt:          of bananas.", has USM coordinates 
technical/biomed/1471-2105-3-6.txt:          bananas ". The matching of the two
```
This example again shows the power of the ignore case becuase I searched for the word `BANANA` in all caps but the output was the files in all lowercase. This demonstrates the power of using the -i because it helps find all instances of the input regardless of the case.
## Option 2: -r
This command can be used like:
```
