# MUST DO

**folders with small amounts of samples should be augmented**

**first do nocall identification (freefield1010) on the data**

**check for duplicate audio files and discard them**

**peak-normalize each 5s segment to 0.25 (by google bird bovalization classifier)**

We want to avoid using 5 second clips that have no birdcall in our train data but are labeled as having some call.

If a recording in the train set is 15 seconds and the label is pigeon it means somewhere in the 15 seconds there was a pigeon call. If we think about how the data was created it seems likely that this 15 second audio clip was taken from a longer recording at some location. When clipping the audio it makes sense that the start and end of the clip would be made near a pigeon call (why would you clip a recording to start 30 seconds before the first birdcall or end 30 seconds after any birdcall). Therefore first 5 seconds and last 5 seconds of any train data seem to be logical choices for less noisy data (but still possible that they have no birdcall).

**https://www.kaggle.com/models/google/bird-vocalization-classifier/TensorFlow2/bird-vocalization-classifier**

**Postprocess: To predict chunk n, the models take 10 seconds: 5 seconds from the chunk n and 2.5 seconds from the previous and next chunks. (top solution)**

**Cross entropy loss**

**efficientnet_b0**

**https://zenn.dev/yuto_mo/articles/ad43c630729073**

**https://www.kaggle.com/competitions/birdclef-2024/discussion/512340**

**https://www.kaggle.com/competitions/birdclef-2024/discussion/511905**



## Maybe useful:
 - https://joblib.readthedocs.io/en/stable/
