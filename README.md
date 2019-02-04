# Finding ET
The inspiration of this fun side project came from: https://www.kaggle.com/tentotheminus9/seti-data

## Aim
The AIM of this side project is to help (past challenge) classify signals that have been converted to **spectrograms**. 

On the first run, I take the already pre-processed images (into spectrograms) to build a learning algorithm **DenseNet201**. The winning team of the 2017 competition achieved **~95%** Accuracy, with second place achieving **~94.6** accuracy. 

On our first attemp we reach **~94.00** Accuracy on a much smaller dataset than what was provided for the competition. 

## About SETI
Over the past few years, SETI have launched a few initiatives to engage the public and ‘citizen scientists’ to help with their search. Below is a summary of their work to date (from what I can tell).

In January 2016, the Berkeley SETI Research Center at the University of Berkley started a program called Breakthrough Listen, described as “the most comprehensive search for alien communications to date”. Radio data is being currently been collected by the Green Bank Observatory in West Virginia and the Parkes Observatory in New South Wales, with optical data being collected by the Automated Planet finder in California. Note that (for now at least), the rest of this description focusses on the radio data.

The basic technique for finding a signal is this; point the telescope at a candidate object and listen for 5 minutes. If any sort of signal is detected, point slightly away and listen again. If the signal drops away, then it’s probably not terrestrial. Go back to the candidate and listen again. Is the signal still there? Now point to a second, slightly different position. How about now? The most interesting finding is, as you might expect, SIGNAL - NO SIGNAL – SIGNAL - NO SIGNAL – SIGNAL.

The Breakthrough Listen project has just about everything covered. The hardware and software to collect signals, the time, the money, and the experts to run the project. The only sticking point is the data. Even after compromising on the raw data’s time or frequency resolution, Breakthrough Listen is archiving 500GB and data every hour (!).

- directly from Kaggle Post

## Future Work
I will use a much larger Dataset provided:  https://github.com/setiQuest/ML4SETI/blob/master/tutorials/Step_1_Get_Data.ipynb  
which contains **35K** images, and compare my results from now!

What I would love to do after is build a webapp, that would allow for anyone to upload the raw *.dat* files, I would convert the raw data into a **spectrogram** and output a classification right through the browser! 