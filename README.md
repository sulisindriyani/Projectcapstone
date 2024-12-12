# ⚙️ Machine Learning Path
Kiddoshine (prediction of stunting in toddlers) uses google colab to predict stunting in children with data inputted by users, this model develops several attributes such as Gender, Age, Birth Weight, Birth Length, Weight, Length, and Breastfeeding which are processed by clarifying the data which will produce an output of toddler health status (stuning or not stunting).<br>

# 📁 Dataset
The data used for our model is in a CSV file named Stunting_Dataset.csv. The file contains attributes such as Gender, Age, Birth Weight, Birth Length, Weight, Length, and Breastfeeding. <br>
We split the dataset into training and testing sets with a ratio of 80:20 to ensure unbiased evaluation of the model.<br>

# 🧰 Requirement
To run the code in this repository, the following dependencies are required:<br>
1. TensorFlow (includes Keras).<br>
2. Pandas.<br>
3. scikit-learn.<br>
4. joblib.<br>
5. Matplotlib.<br>
6. numpy.<br>
7. google colab.<br>

# 🧬 Arsitektur Model
Our model architecture uses the integration of Random Forest with the bagging method to produce a more robust and precise classification model. <br>
By utilizing 100 trees in Random Forest as well as 10 models in the bagging process, this architecture is designed to handle variability in data and provide more stable results.<br>

# 🏋️‍♂️ Training
Our model was trained using the bagging technique with the command bagging_model.fit(X_train, y_train).<br>
The training process was performed on the training set (X_train and y_train) by taking random subsets of the data using the bootstrap technique.<br>
The base model is trained on each subset simultaneously. Once all the base models are trained, their prediction results are combined to improve accuracy and reduce variance. Thus, the models produce more stable and reliable predictions.<br>

# 📝 Evaluation
After training, the model is evaluated on a test set to measure its performance. Following the evaluation of the model before the model is saved, the evaluation is reported:<br>
Akurasi Model: 0.854
Laporan Klasifikasi:
              precision    recall  f1-score   support

           0       0.71      0.49      0.58       409
           1       0.88      0.95      0.91      1591

    accuracy                           0.85      2000
   macro avg       0.79      0.72      0.75      2000
weighted avg       0.84      0.85      0.84      2000


# 💾 Saving the Model
The trained model is stored in two formats:<br>
1. modelstuntingrf.pkl: The model is saved in .pkl format using the joblib.dump(bagging_model, 'modelstuntingrf.pkl') function.<br>
( file : https://drive.google.com/file/d/1SlwAl8hsQ75vYxnydWm5TAwEmEetATC5/view?usp=drive_link )<br>




