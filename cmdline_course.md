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
* mv 
* cat 
* less 
* cp 
* rm 
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
My solution didn't count 18 words like Adéle AINO and all the ä ö å words. The second command exports the result into a file:
```
egrep "\b(A|a)[-a-z]*\b" katinka_rabe.word_list.txt > Aardvark.txt
```

## Week 4
Processing texts, regular expressions.

This is Stephen Cole Kleene, who invented them:  
![Picture of Stephen Cole Kleene](https://en.wikipedia.org/wiki/Stephen_Cole_Kleene#/media/File:Kleene.jpg)

## Week 5
Scripts make live simpler and bring joy!

## Week 6
Program installations, nothing more to say... But _make_ command is great!

## Week 7
Version Control, I think I liked it.

## Week 8 (Time goes fast...)
GitHub, Jekyll and Final Project... basically everything that you see here.

The final thing I have to do (hopefully), is to merge the branch I used to write this text with the main site (lets call it so... no need to go into details)
```
git checkout master
```
and then:
```
git merge cmdline_course
```
and then push! And that's pretty much all!

## And last, but not least:

Course | Year | My Opinion
--- | --- | ---
*Command-Line Tools for Linguists* | `2023` | **GREAT!**




