# Machine Learning Path
Kiddoshine (prediction of stunting in toddlers) uses google colab to predict stunting in children with data inputted by users, this model develops several attributes such as Gender, Age, Birth Weight, Birth Length, Weight, Length, and Breastfeeding which are processed by clarifying the data which will produce an output of toddler health status (stuning or not stunting).<br>

# Dataset
The data used for our model is in a CSV file named Stunting_Dataset.csv. The file contains attributes such as Gender, Age, Birth Weight, Birth Length, Weight, Length, and Breastfeeding. <br>
We split the dataset into training and testing sets with a ratio of 80:20 to ensure unbiased evaluation of the model.<br>
accuracy of the trained model: <br>
![image](https://github.com/user-attachments/assets/256e1446-72e2-4d1a-963b-3b4300147edd)


Confusion Matrix of the trained model: <br>
![image](https://github.com/user-attachments/assets/26dffc64-e2e9-4b06-8df3-5adc755109ef) 

# Requirement
To run the code in this repository, the following dependencies are required:<br>
1. TensorFlow (includes Keras)
2. Pandas
3. scikit-learn
4. joblib


# Saving the Model
The trained model is stored in two formats:<br>
1. modelstuntingrf.pkl: The model is saved in .pkl format using the joblib.dump(bagging_model, 'modelstuntingrf.pkl') function.<br>
( file : https://drive.google.com/file/d/1SlwAl8hsQ75vYxnydWm5TAwEmEetATC5/view?usp=drive_link )<br>
2. model_stunting.h5: The model is converted into H5 format using the function model.save('model_stunting.h5') <br>
( file : https://drive.google.com/file/d/1iJK2vStgPD9GcGu0cyS4dIMMzikvRYQX/view?usp=sharing )<br>


Once the model is trained, we then connect the output classified image into a database containing information on stunting prediction. The output will then be the information gathered from the database.<br>



