# Match Winner Prediction

Below is the excerpt from the MachineHack website for MachineHack’s ODI Match Winner: Weekend Hackathon #9 [Link To Their Website](https://www.machinehack.com/hackathons/odi_match_winner_weekend_hackathon_9)

### **Problem Statement & Description:**

Our country shares a great deal of history with the game of cricket. Introduced as a royal game by the British during the British Raj, India took on the game as a popular sport even after its Independence. Today cricket is more than just a sport in India. In this hackathon, we challenge data science enthusiasts to predict the winning team of an ODI (One Day International) match.

Given are 9 distinguishing factors that can influence the outcome of a cricket match. Your objective as a data scientist is to build a machine learning model that can accurately predict the winning team of an ODI match.

### **Data Description:-**

The unzipped folder will have the following files.

* Train.csv –  2293 observations.
* Test.csv –  983 observations.
* Sample Submission – Sample format for the submission.
* Target Variable: MatchWinner

### **Evaluation**

The leaderboard is **evaluated using multi-class log loss** for the participant’s submission.



# Program Setup

The program loads data and performs EDA to normalize the data.
It uses a Random Forest Classifier method with Hyperparameter tuning using randmized search followed by grid search.
Subsequently, we use the Feature Importance attribute of RFC to identify the top relevant features and see if we can achive better results with reduced features.

Please note that the program provides an output of the model, however, due to absence of labels for the test dataset, it is not possible to verify the accuracy of results with the test data. The rfc_temp.xlsx file gives the output using all the features of the dataset, while rfc_reduced_temp.xlsx gives the output from using only the relevant features from the data.
