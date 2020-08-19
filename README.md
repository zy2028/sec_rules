# sec_rules

This repository tracks manual changes on rule texts

## Folders

/raw and /formatted both contain pre-processed rule texts, potentially have some incorrect headings

We’ll be working on files under /formatted and update them accordingly. /raw folder will be kept as a reference.

## Files

Rule files are named release_no.txt, for example, 33-10450.txt

Each rule is organized as follows:

1. URL of original pdf file

2. Pre-processed Table of Contents, to be compared with the originals. Ends with “<END TABLE OF CONTENTS\>"

3. Header, includes title and author of the rules. Ends with “<END HEADER\>"

4. Main Text, include main texts of the rules, to be corrected. Ends with “<END MAIN TEXT\>”

5. Footnotes. 

Part 1 and 2 are for reference only and should be deleted after correction. See below **How to Correct**. 

## What to Correct

We'll be focusing on correcting **wrong Table of Content items**

While pro-processing with codes, some **texts** were incorrectly identified as **headings**. 

For example, text "...see rule 305. A. for reference" could be identified as 

...see rule 305. 

**<h\>A. for reference</h\>**

The part after A. was incorrectly recognized as a heading

## How to Correct

First, open the original pdf file of the rule. They usually have a Table of Content section before the main text.

Then, compare the Table of Content section in the text file with the pdf file. There could be **incorrect** headings or **missing** headings.

For incorrect headings, please find the location in the main text and delete the <h> </h> tags before and after the paragraph

For missing headings, please insert <h\> </h\> tags before and after the paragraph

ALL CHANGES should be done in the main text instead of the Table of Contents.

After correction, **DELETE** "<END TABLE OF CONTENTS\>" and everything above it.
  
While correcting Table of Contents, please disregard everything after "ECONOMIC ANALYSIS" or "PAPERWORK REDUCTION ACT". Our main focus is usually on Section II. 
  
I have already formatted formatted/2018/33-10450.txt

## Git Basics

TBA
