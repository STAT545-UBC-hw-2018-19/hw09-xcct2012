make-activity
=============

The commit history of this repository reflects what a student might do as she works through [this activity](http://stat545-ubc.github.io/automation04_make-activity.html) from [STAT 545](http://stat545-ubc.github.io). This fully developed example shows:

  * How to run an R script non-interactively
  * How to use `make`
    - to record which files are inputs vs. intermediates vs. outputs
    - to capture how scripts and commands convert inputs to outputs
    - to re-run parts of an analysis that are out-of-date
  * The intersection of R and `make`, i.e. how to
    - run snippets of R code
    - run an entire R script
    - render an R Markdown document (or R script)
  * The interface between RStudio and `make`
  * How to use `make` from the shell
  * How Git facilitates the process of building a pipeline
  
 # STAT547_hw09
 ## Zachary Sherker

This is a repository for Zachary Sherker's STAT547 hw 9.

## In this assignment, I will:

Add one R. script and one .Rmd script to Jenny Bryan's Makefile activity (found here: https://github.com/STAT545-UBC-students/hw09-xcct2012/blob/master/Makefile). My additions to Jenny's Makefile create an analysis of the frequency of letters used in the word.txt file (found here: https://github.com/STAT545-UBC-students/hw09-xcct2012/blob/master/word_histogram/words.txt) and outputs a histogram (found here: https://github.com/STAT545-UBC-students/hw09-xcct2012/blob/master/word_histogram/letters_freq.png) and a table summarizing this data for each letter (found here: https://github.com/STAT545-UBC-students/hw09-xcct2012/blob/master/word_histogram/letters_freq.tsv) using the following R script (found here: https://github.com/STAT545-UBC-students/hw09-xcct2012/blob/master/word_histogram/letter_frequency.R) and Rmd. file (found here: https://github.com/STAT545-UBC-students/hw09-xcct2012/blob/master/word_histogram/letters_freq.Rmd).

All files can be found in the following word_histogram folder:

https://github.com/STAT545-UBC-students/hw09-xcct2012/tree/master/word_histogram
