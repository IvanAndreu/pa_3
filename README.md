---
title: "pa_3"
author: "Yo"
date: "4/1/2022"
output: html_document
---

# Questions 
7
**A* 
The first two lines get the values of the onset and the offset of the vowels, the third line, defines duration, which is the difference between the offset and the onset. On the second portion of the code, we see something similar to what we saw on Jacewicz (2011). The idea of calculating the (20%, 35%, 50%, 65%, 80%) is obtaining time landmarks at those percentages of the total duration. By obtaining these values, we can later see the evolution of the vowel at those 5 points, giving as a better account of the vowel development. 

**B**
First a .cvs file is created, later, a loop is set. The code sets the path to the folder where the stimuli files are stored, the code instructs to gets the .wav file, create strings for .wav file, read the .wav file and the textgrid. After this, it checks the intervals in the textgrid, sets default values, and adds a string variable for the given personal id provided. 
In the last chunk the code goes through the loop getting the labels of the intervals, then it gets the onset and offset of the given intervals, then it gets the item and vowel labels, along with the language label. The code then instructs to calculate the vowel onset and offset as the duration of the vowels. After this it calculates the landmarks in (20%, 35%, 50%, 65%, 80%), gets the formants, and calculates spectral centroids and trajectory length. Finally, it prints the results and saves them in the .CVS file

**C**
The main difference between both assignments was the number of files that we manipulated, in this sense, the main change comes with the main advantage; the less files we manipulate, the less time consuming it is. Additionally, by having everything in one file it might be easier to keep track of the file, and not losing spare files on the process. 
Regarding the disadvantages, we can attend to a limited amount of audio time that Praat can process, meaning that if we have a .vaw that is too long, we might need to split it. 


## Load libraries and data

```{r, libs, message=F, warning=F}
library(tidyverse)
library(untidydata)
library(ggplot2)
library(readr)
```

```{r, load-data}
library(readr)
vowel_data <- read_csv("pa_3/data/vowel_data.csv")
View(vowel_data)
```


```{r}
mean(df$f1_cent)
sd(df$f1_cent)
```











