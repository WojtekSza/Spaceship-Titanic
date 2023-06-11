# Kaggle Spaceship Titianic commpetition
Competition details can be found here 
```
https://www.kaggle.com/competitions/spaceship-titanic/
```
<img src="https://github.com/WojtekSza/Real_time_machine_learning/blob/main/Real_time_ml/4.jpg" alt="spark" width="800"/>  <br>

Then we will upload "train" and "test" datasets downloaded from Kaggle webpage <br>
Data set will be limited to text of Twitters only (w/o location and key features). <br>
<img src="https://github.com/WojtekSza/Real_time_machine_learning/blob/main/Real_time_ml/5.jpg" alt="spark" width="800"/>  <br>

For machine learning we will use Classification in the Azure Automated ML: <br>
<img src="https://github.com/WojtekSza/Real_time_machine_learning/blob/main/Real_time_ml/6.jpg" alt="spark" width="800"/>  <br>
For the tutorial purpose there was selected Random Forest model with 30-70% training data split <br>

After 30 minutes model is trained with following results:<br>
<img src="https://github.com/WojtekSza/Real_time_machine_learning/blob/main/Real_time_ml/10.jpg" alt="spark" width="800"/>  <br>
## Accuracy 77% w/o any specific model adjustement of alghorithm selection. Not bad! (Precision and recall at the same level).

Final step to verify results on Kaggle with predicted classes in test.csv file: <br>
<img src="https://github.com/WojtekSza/Real_time_machine_learning/blob/main/Real_time_ml/9.jpg" alt="spark" width="800"/>  <br>
Nice. Verified results shows 76% accuracy<br>

# Conclusion
With usage Azure Automated Machine Learning we can quickly train model w/o any code with good initial accuracy. Verification of results shows good correlation 77% vs 76%. Further tune up of model paramters for sure will improve result.

# Last step is to remove all created resources
```
az group delete --name Realtimeml
```
