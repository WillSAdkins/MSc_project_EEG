# Learning to read the mind: Decoding of inner and imagined speech from EEG signals via Machine learning

This page contains the code for the analysis performed in my final year project/dissertation for MSc Data Science at the University of Bath. 

Mode of Stimuli : The manner in which the stimulus (word prompt) is expressed to participants. i.e. An image, sound, text representation ...

In this work EEG data was recorded for 9 participants in which 4 participants performed inner speech, and 5 imagined speech of 4 healthcare related words (Ambulance, Hospital, Clock and Lamp). Our work for the experimental paradigm used in data collection can be found at https://github.com/Mithrandir98/BCI_paradigm.

This work challenges the seemingly tacit assumption that mode of stimuli used in stimulus stages of recording structures is unimportant in collecting high quality EEG data, and the aim of the investigation was to understand the infleunce on the success of decoding inner and imagined speech, of mode of stimuli/representation used when prompting what to speak/imagine in the data collection stage. This was tested by alternating between the use of Visual/image, text and audio representations when prompting participants what to speak/imagine in the case of each of our 4 words during recordings. Three different classification setups were used in experiments, with research questions:
1. Does mode of stimulus affect the success with which speech can be decoded, in terms
of 4-way classification accuracy between the 4 words.
2. Does mode of stimulus affect the success with which the speech of monosyllabic vs
trisyllabic nouns can be decoded, in terms of binary classification accuracy (Ambulance and Hospital vs Clock and Lamp).
3. Does mode of stimulus affect the success with which speech can be decoded for nouns
with vowels /æ/ vs /6/, in terms of binary classification accuracy (Ambulance and Lamp vs Hospital and Clock).

For this both deep neural networks and random forest models were trained to perform classification in the 3 different cases and results of this can be seen in the below tables.

![image](https://user-images.githubusercontent.com/81915637/201978848-662de4df-c8ff-45ca-b6b3-0fb7e63c8421.png)

![image](https://user-images.githubusercontent.com/81915637/201978961-8a9e5443-70e8-46b7-9fa5-955a26f6eeaf.png)

![image](https://user-images.githubusercontent.com/81915637/201979039-b9b81937-46b9-408a-b71f-894b93a2682a.png)

Results suggested that mode of stimuli used in the stimulus stage of recordings does not influence the ability to decode subsequent inner or imagined speech (in any of the 3 cases). Moreover, the random forest algorithm appeared to largely outperform the deep neural network, either suggesting that the danger of overfitting is worse for the random forest or the ability to decode speech imagery is better, with the former being the most likely given some problems with the data. However it was found that models performed better on the task of decoding inner speech, with an explanation based off methods applied in this work not found.
