# Machine Learning Path
Kiddoshine utilized google colab to predict stunting in children by developing several attributes such as Gender, Age, Birth Weight, Birth Length, Body Weight, Body Length, and Breastfeeding. <br>

# Dataset
The dataset used for training data is Stunting_Dataset.csv which contains the following attributes: Gender, Age, Birth Weight, Birth Length, Body Weight, Body Length, and Breastfeeding.<br>
This dataset was collected from kagle and divided into a training set and a testing set with a ratio of 80:20.<br>
accuracy of the trained model: <br>
![image](https://github.com/user-attachments/assets/256e1446-72e2-4d1a-963b-3b4300147edd)


Confusion Matrix of the trained model: <br>
![image](https://github.com/user-attachments/assets/26dffc64-e2e9-4b06-8df3-5adc755109ef) 


# Saving the Model
The trained model is stored in two formats:<br>
1. modelstuntingrf.pkl: The model is saved in .pkl format using the joblib.dump(bagging_model, 'modelstuntingrf.pkl') function.<br>
( file : https://drive.google.com/file/d/1SlwAl8hsQ75vYxnydWm5TAwEmEetATC5/view?usp=drive_link )<br>
2. model_stunting.h5: The model is converted into H5 format using the function model.save('model_stunting.h5') <br>
( file : https://drive.google.com/file/d/1iJK2vStgPD9GcGu0cyS4dIMMzikvRYQX/view?usp=sharing )<br>


Once the model is trained, we then connect the output classified image into a database containing information on stunting prediction. The output will then be the information gathered from the database.<br>



