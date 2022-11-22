# AV-job-a-thon-november-2022

### Competition hosted on <a href="https://datahack.analyticsvidhya.com/contest/job-a-thon-november-2022/#About">Analyticsvidhya</a>

# About

### Build a machine learning/deep learning approach to forecast the total energy demand on an hourly basis for the next 3 years based on past trends.

### Initially, I thought a machine learning approach itself was enough to handle any time-series-based problem but this competition has proved that I was totally wrong.

### In one of the previous time-series-based competitions, I used the boosting regressor model and it gave me a good leaderboard rank. I tried the same approach in this competition and it become a major blunder and had given the worst rank in the private leaderboard.

### The machine learning-based approach didn't learn signals or patterns from the train data, the model learned only noise from the data.

### Finally, for this problem, the boosting algorithm well performed on the train data and failed to generalize on the test data(Overfitting!).

### I had tried the seasonal decomposing linear model and it performed better than the boosting model.

### Final Competition score is 583.858113004428

### Leaderboard Rank is 207

### Evaluation Metric is RMSE.

### File information
 
 * av-job-a-thon-november-2022-eda.ipynb [![Open in Kaggle](https://img.shields.io/static/v1?label=&message=Open%20in%20Kaggle&labelColor=grey&color=blue&logo=kaggle)](https://www.kaggle.com/hari141v/av-job-a-thon-november-2022-eda)
    #### Basic Exploratory Data Analysis
    #### Packages Used,
        * seaborn
        * Pandas
        * Numpy
        * Matplotlib
* av-job-a-thon-november-2022-model.ipynb [![Open in Kaggle](https://img.shields.io/static/v1?label=&message=Open%20in%20Kaggle&labelColor=grey&color=blue&logo=kaggle)](https://www.kaggle.com/hari141v/av-job-a-thon-november-2022-model)
    #### Data Pre-processing and model. 
    #### Packages Used,
        * Sklearn
        * Pandas
        * Numpy
        * Matplotlib
        * Lightgbm
        * shap
     #### Created light gradient boosting regressor model and evaluated with RMSE. 
     #### [For more detailed information about the model.](https://github.com/hariprasath-v/AV-job-a-thon-november-2022/blob/main/Approach_AV_job_a_thon_November_2022.pdf)
     

### Lightgbm Model Feature Importances
![Alt text](https://github.com/hariprasath-v/AV-job-a-thon-november-2022/blob/main/Model%20Visualization/Lightgbm%20regressor%20top%20feature%20importances.png)

### SHAP Lightgbm Model Feature Importances
![Alt text](https://github.com/hariprasath-v/AV-job-a-thon-november-2022/blob/main/Model%20Visualization/SHAP%20Lightgbm%20regressor%20top%20feature%20importances.png)

### SHAP Top feature impact the model
![Alt text](https://github.com/hariprasath-v/AV-job-a-thon-november-2022/blob/main/Model%20Visualization/SHAP%20-%20Top%20feature%20impact%20the%20model.png)

### SHAP Top feature influences the single observation
![Alt text](https://github.com/hariprasath-v/AV-job-a-thon-november-2022/blob/main/Model%20Visualization/SHAP%20-%20Feature%20impact%20the%20single%20obsevartion.png)

### Energry Demand for Next 3 Years
![Alt text](https://github.com/hariprasath-v/AV-job-a-thon-november-2022/blob/main/Model%20Visualization/Train%20and%20Test%20plot.png)
