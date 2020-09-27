# Birdsong Dataset
Recorded during COVID-19 Quarantine

In the foothills of the Carson Range, within the Sierra Nevada Mountains, we captured footage and audio from a motionactivated wildlife camera. The camera was trained on bird feeders and the surrounding area, and captured eleven second video and audio samples (44.1 kHz). The birds recorded included Quail, Blue Jays, Black Headed Grosbeaks, Doves, Robins, Red Finches, Stellars Jays, Black-billed Magpies, Yellow Warblers and Varied Thrush, among others. We extracted the audio from the captured video and resampled it to a 22 kHz sample rate. This data was collected during the time period of 'COVID quarantine' in Nevada, March, April and May of 2020, at a time of paricularly low environmental car and airplane noise.  This dataset complements the paper 'Using Self-Supervised Learning of Birdsong for Downstream Industrial Audio Classification' presented at ICML 2020 Workshop on Self-supervision in Audio and Speech on July 17, 2020. https://openreview.net/forum?id=_P9LyJ5pMDb

Within the 'raw-audio-unfiltered-22000-sample' folder are the individual audio recording data arrays.  These recordings have been resampled at 22000 and the raw data vector is stored as individual csv's.  Recordings are all approximately ten seconds long.  As github limits directories to 1000 files, the training set is split into two directories.

In the 'notebooks' folder you will find the script used to strip and downsample the audio from the original captured video.

This dataset complements the repository here https://github.com/SingingData/Birdsong-Self-Supervised-Learning.  

This dataset is unfiltered.  We recommend filtering this dataset before using.  There are two notebooks to preprocess and filter this birdsong available here https://github.com/SingingData/Birdsong-Self-Supervised-Learning/tree/master/Notebooks/Preprocessing.  The first eliminates those audio samples with a low differential between minimum and maximum magnitude.  The second method performs a K-means analysis on the Constant Q transform of the audio sample to identify and eliminate unwanted samples. 
