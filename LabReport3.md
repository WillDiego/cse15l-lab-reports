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
$ grep "BANANA" -i technical/biomed/*.txt
technical/biomed/1471-2105-3-6.txt:          fond of bananas." and "I am of very fond bananas. Am I a
technical/biomed/1471-2105-3-6.txt:          of bananas.", has USM coordinates 
technical/biomed/1471-2105-3-6.txt:          bananas ". The matching of the two
```
This example again shows the power of the ignore case becuase I searched for the word `BANANA` in all caps but the output was the files in all lowercase. This demonstrates the power of using the -i because it helps find all instances of the input regardless of the case.
## Option 2: -r
This command can be used like:
```
$ grep "asparagus" -r technical/            
technical/government/About_LSC/commission_report.txt:typically work in Yakima from the April asparagus harvest through
```
This example demonstrates the -r command which recursively searches through all of the files in a directory (and all sub directories). This is a good demonstration becuase in the argument it can be seen that I just put in the directory `technical/` and no files yet there was a file output. This demonstrates that the grep command went through every single file and checked if there was an occurance of the word `asparagus`.
```
$ grep "amazing" -r technical/
technical/911report/preface.txt:                the American people and their amazing resilience and courage as they fought back. We
technical/biomed/1471-2180-3-10.txt:        differences between these genomes with amazing detail.
technical/biomed/1471-2350-3-12.txt:        amazingly consistent for fold change and direction of
technical/biomed/1471-2350-3-12.txt:        not used on the GeneChip ®analysis revealed amazing
technical/biomed/gb-2003-4-5-r34.txt:        showed that the infinite mixture approach works amazingly
technical/government/Media/Rental_rules.txt:"It's pretty amazing how many elected officials aren't even
technical/government/Media/Service_Agency.txt:amazing how many people call us up the day before or after their
technical/plos/journal.pbio.0020012.txt:        … but we put them onto yeast, justbeing the simplest model, and amazingly [they] did what
technical/plos/journal.pbio.0020035.txt:        amazing array of so-called secondary metabolites that have evolved to give their producers
technical/plos/journal.pbio.0020262.txt:        (mirror-reversed organs) and succumbs to laughter at the sight of Ditto, the amazing
technical/plos/journal.pbio.0020311.txt:        degree. A single hormone can regulate an amazingly diverse array of cellular and
```
This is another good example becuase it shows again how only the `technical` directory was used but so many files were found. Therefore demonstrating that there was some recursion when findind the files.
## Option 3: -w
This command can be used like: 
```
$ grep "ban" -w technical/biomed/*.txt
technical/biomed/1471-2091-2-12.txt:        microbial pathogen outbreak, inspired a governmental ban on
technical/biomed/1472-6963-3-1.txt:          after the ban, noncitizens must not receive public
```
The `-w` is a command that only takes instances of the whole word not occurances inside of a word. This can be seen in the example because only the word ban shows up not other words such as banana. As shown earlier there were infact files in the biomed folder that contained the words banana so this shows that only the word that is only `ban` is shown.
```
$ grep "ban" -w technical/911report/*.txt
technical/911report/chapter-13.3.txt:                they concluded that killing Bin Ladin did not violate the assassination ban
technical/911report/chapter-13.4.txt:                location, the CIA might have violated the assassination ban. Tenet did not recall
technical/911report/chapter-3.txt:                increased. A proposal to ban knives altogether in 1993 had been rejected because
technical/911report/chapter-6.txt:                the assassination ban. Hence, Massoud was told not to take any such action without
technical/911report/chapter-6.txt:                the ban on assassinations in Executive Order 12333. The big issues-who would pay for
```
This is another good example with a different directory. It shows the same result that only the files contating `ban` are shown, not any files contating a word that includes ban.
## Option 4: -l
This command can be used like:
```
$ grep "ban" -l  technical/911report/*.txt
technical/911report/chapter-1.txt
technical/911report/chapter-10.txt
technical/911report/chapter-11.txt
technical/911report/chapter-12.txt
technical/911report/chapter-13.1.txt
technical/911report/chapter-13.2.txt
technical/911report/chapter-13.3.txt
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-2.txt
technical/911report/chapter-3.txt
technical/911report/chapter-5.txt
technical/911report/chapter-6.txt
technical/911report/chapter-7.txt
technical/911report/chapter-8.txt
technical/911report/chapter-9.txt
```
The -l lists only the file paths of the files that contaion the instance of `ban`. So in this case all the files listed contain an occurance of `ban` however we do not see where it is found becuase that is what -l hides.
```
$ grep "guy" -l  technical/911report/*.txt
technical/911report/chapter-1.txt
technical/911report/chapter-3.txt
technical/911report/chapter-5.txt
```
This is another example that shows all the files that contain the word `guy`. This demontrates that only 3 files in all of the 911report contain the word `guy`.




Apologies if the code breaks were cut off. The formating of printing caused some of them not to wrap and get cut off.
If you'd like a link to the webpage itself it can be viewed here: https://willdiego.github.io/cse15l-lab-reports/LabReport3.html
