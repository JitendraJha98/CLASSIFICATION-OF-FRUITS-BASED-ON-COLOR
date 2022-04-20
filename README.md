# CLASSIFICATION-OF-FRUITS-BASED-ON-COLOR

1.INTRO

Fruit quality is important since it is utilised in a number of applications such as export, fruit jam production, and fruit juice production. The fruit business is critical to a country's economic development. Fruit classification and quality assessment is currently a key study topic in the mechanised world. The main focus of this project is on a cost-effective method of analysing the quality of fruits based on colour, shape, and size.
Here we use different classification models for classification of fruits.

As dataset Contains many Columns such as 'fruit_label', 'fruit_name', 'mass', 'width', 'height', 'color_score'. Among them fruit name Column is one dependent variable. Which indicates that the 4 different types of fruits.
So here the output or target value will be four different types of fruits names. so it is a classification problem.
So here we can use K- nearest neighbor Classifier for initial classification.
KNN is a non-parametric and lazy learning algorithm. Non-parametric means there is no assumption for underlying data distribution. In other words, the model structure determined from the dataset. This will be very helpful in practice where most of the real-world datasets do not follow mathematical theoretical assumptions. Lazy algorithm means it does not need any training data points for model generation. All training data used in the testing phase.



2.1 DATASET BREIFING




There is total 59 observations in data set. There is total seven columns out of which six columns are independent variable. Here, except 'fruit name' Column all other columns are independent. Fruit name' is dependent variable which is indicating that the four different types of fruits.
<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164286758-93dd88dd-73de-490d-b710-b0bc9dc580f0.png">








2.2 EDA

To get maximum insights of data we performed EDA which uncovered the underlying structure and distribution of data.
To begin, we created a histogram to visualise the data distribution. We can see how the data in different columns varies.

After that, we plotted pair plot to analyze the relationship of dependent variable i.e., fruit name with different features present in the dataset.
<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164286899-bb87bf3a-a691-486e-8cc6-780a53447e9a.png">


2.3 Feature Selection

After analysing the relationship, we attempted to extract a feature that we might utilise to create a more accurate prediction model. We used a heatmap to identify the association between different factors in order to achieve this goal.
<img width="348" alt="image" src="https://user-images.githubusercontent.com/72140481/164286927-c7a3aadb-f498-4ee6-8785-46d514065129.png">

	

Here, data has only six independent variable which has linear correlation with dependent variable.
If there are more than one independent variable, not all independent variables contribute equally in estimation of dependent variable. This can be quantified using correlation between dependent and independent variable.
<img width="342" alt="image" src="https://user-images.githubusercontent.com/72140481/164286957-2b8268fc-1a71-4c2f-9f2c-feb5e6085c7b.png">

	
We chose all of the columns for the prediction model because we can see that there isn't any association between the different features. After that we classified the dependent variables into different labels.
For apple it is 1, for mandarin it is 2. for orange it is 3 and for lemon it is 4. Now we will visualize this data on plots for further exploration.
<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164286785-f7477bb6-40c6-4f8c-bb2b-bf2950306725.png">
<img width="378" alt="image" src="https://user-images.githubusercontent.com/72140481/164286986-3d928961-7f16-435f-867f-4329e2611d5c.png">
<img width="371" alt="image" src="https://user-images.githubusercontent.com/72140481/164287000-df304b0d-ec83-49db-99a0-f3578d1bcc07.png">







2.3 Train Test Split
Following feature selection, we separated the entire dataset into train and test datasets, with 1/3 used for testing and the remaining 2/3 for training.

<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287026-bd1a193c-3f9b-4c33-8899-1cf92bd68d27.png">


2.4 Classification Models

After splitting the dataset into train and test datasets we used K-Nearest Neighbors classifier to predict a new record on the basis of this data. For classification purpose we are using 10 distinct values at a time.

After training the model we calculated the score and found that it is coming 100% for train dataset and 60% for test dataset.

	    <img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287053-b0006acb-cbb5-4511-ab2a-c25a3cfedbc5.png">
<img width="317" alt="image" src="https://user-images.githubusercontent.com/72140481/164287075-90eab51f-66e9-478b-88ca-34384973c583.png">


Following is the classification report of the prediction model we trained.

<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287092-704656ca-56fa-4201-b3cd-cc232b8548b3.png">



We have also used other algorithms to train our data and the prediction scores of other models are following:
2.5.1 Support Vector Machine Algorithm
<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287111-6deae5a6-bbd8-46c5-8fda-6773cced96f8.png">

2.5.2 Decision Tree Classifier

<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287126-fd84dcfa-472f-466a-9972-a8ff83bee606.png">




2.5.3 Naive Bayes Algorithm

<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287139-f00a16d9-a9cd-4bf2-ac8f-c497bc1b7851.png">

2.5.3 Random Forest Classifier

<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287151-ae04f926-dbbf-4e2f-a480-59a76d2d4be9.png">






2.Results and prediction


Different classification model analysis on same dataset

Finally, we selected K- nearest neighbor Classifier for classification. As KNN is a non-parametric and lazy learning algorithm. Non-parametric means there is no assumption for underlying data distribution. In other words, the model structure determined from the dataset. This will be very helpful in practice where most of the real-world datasets do not follow mathematical theoretical assumptions. Lazy algorithm means it does not need any training data points for model generation. All training data used in the testing phase.
Which is further supported by the following statistics and results.

<img width="430" alt="image" src="https://user-images.githubusercontent.com/72140481/164287178-f7acb093-56b4-4d29-9a99-123212ea85ca.png">




STATISTICS
<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287189-168fe2bd-46b1-4261-be8c-e37bc4fea24f.png">


Result
<img width="416" alt="image" src="https://user-images.githubusercontent.com/72140481/164287207-68194120-1711-448a-938a-92d52854a909.png">

