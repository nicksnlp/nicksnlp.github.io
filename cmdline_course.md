---
layout: default
---

## About the course
A nice introduction to the command line and basic programming environment.  
   
As this was my first course, it was also a good intro to learning at Helsinki University in general, the self-assisted learning style and the assignments/grading system.

## Week 1
Basic intro.  
Well, the first week teaches you to walk, and to navigate your system, using command line and the pipeline e.g.:  

```
cat file.txt | sort
```
It displays a file on the screen, and sorts the lines alphabetically.

I've learned, among other things:
* ls
* pwd
* whoami
* wget
* mv 
* cat 
* less 
* cp 
* rm 
* rm -R
* mkdir 
* cd

## Week 2
I would call it Intro 2, similar to week 1, but slightly deeper, work with remote server introduced.  
I have created a configuration file to connect to it.  
First I've learned how to show the hidden files:
```
ls -a
```
Then created a file called config. I used nano, I didn't like emacs. First typed:
```
cd .ssh   
```
Then:
```
nano config 
```
And it will create a file, I filled it then with some info.

## Week 3
Getting hands on texts. I have made some long pipelines here :). It was nice. It's a pity that I didn't know that you could do several attempts for the exercises, because I have forgotten about some letters while processing texts.
```
egrep "\b(A|a)[-a-z]*\b" katinka_rabe.word_list.txt | wc -w
```
My solution didn't count 18 words like Adéle, AINO and all the ä-, ö-, å-words. The second command exports the result into a file:
```
egrep "\b(A|a)[-a-z]*\b" katinka_rabe.word_list.txt > Aardvark.txt
```
Just as an example.

## Week 4
Processing texts, regular expressions (well, they were introduced indeed the week before, but it was more use of them here).

This is Stephen Cole Kleene, who invented them:  
![Picture of Stephen Cole Kleene](https://upload.wikimedia.org/wikipedia/commons/1/1c/Kleene.jpg)  

### tr, sed, grep

**tr** is nice, but **sed** is even nicer, as it substitutes patterns with something else. Of course, *sed -E* brings even more opportunities, especially as combined with *grep*.

```
sed 's/^$/#'
```
will change all the empty lines into hash-tags.  
## Week 5
Scripts make live simpler and bring joy!  
This is the one I made:
```
#! /bin/zsh

ls -sR -1 $1 | 
sort | 
egrep '[[:digit:]] .*\.' | 
uniq -c | 
sort -r | 
grep -vE '^[[:blank:]]+[1] .*'
```
I have also learned how to change permissions (**chmod** command), and how to change my _.zshrc_ file. To change the PATH variable, to add aliases...

## Week 6
Program installations, nothing more to say. The virtual environment appeared to be useful later on... The _make_ command is great! Just type
```
make
```
into command line and it will do the magic (as well as pull out some scripts from src folder)! 

## Week 7
Version Control, I think I liked it. This [video](https://youtu.be/HVsySz-h9r4) explains everything.

I've learned how to deal with git:
```
git clone
```
to make a repository
```
git init
```
to track changes
```
git add
git commit
git push
```
(of course with some arguments!)

and the workflow overall...

## Week 8 (Time goes fast...)
GitHub, Jekyll and Final Project... basically everything that you see here.

The final thing I have to do (hopefully), is to merge the branch I used to write this text with the main site (lets call it so... won't go into details)
```
git checkout master
```
and then:
```
git merge cmdline-course
```
and then push! And that's pretty much all!

## And last, but not least:

Course | Year | My Opinion
--- | --- | ---
*Command-Line Tools for Linguists* | `2023` | **GREAT!**




