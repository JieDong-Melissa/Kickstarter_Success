
# Predicting Kickstarter Crowdfunding Success: Data-Driven Investment Strategies 
![image](https://github.com/JieDong-Melissa/Kickstarter_Success/blob/main/images/kickstarter_image.jpeg)
[Kickstarter](https://www.kickstarter.com/), a global crowdfunding platform launched on April 28, 2009, supports funding for creative projects across various categories such as films, games, music, art, design, and technology. Based in Brooklyn, New York, it operates on an all-or-nothing model, charging backers only if the funding goal is reached. Successful projects offer backers unique rewards.


This dataset includes information on 20,632 Kickstarter campaigns up to February 1, 2017. It contains 59 features detailing various aspects of each campaign, such as campaign ID, project category, subcategory, goal amount, pledged amount, campaign state, launch date, end date, and other relevant metrics. These features provide insights into the performance and characteristics of Kickstarter campaigns, which can be useful for analyzing trends and identifying factors that contribute to campaign success


  
Then our goal will be to evaluate and explore multiple supervised machine learning models, to predict if a project funding will be successful or failed before it is launched. 


This dataset contains data on 20,632 Kickstarter campaigns on the site as of February 1st 2017. There are 59 features

Important attributes are described below:

Project: a finite work with a clear goal that you’d like to bring to life (aka campaign)
Funding goal: amount of money that a creator needs to complete their project
Name: name of project on Kickstarter
Blurb: the short description displayed under the name of your project and on the browse page
Pledged and backers: amount of money that a project has raised and people that have supported it at the point of the API pull
State: successful, failed, cancelled, live or suspended
Deadline, state changed, created at, launched at: deadline given for successful funding, state changed when campaign went to success or failure, time the project was created at, time the project was launched at
Other attributes in this dataset: country, currency, category
To attain a deeper understanding of our data and to have more attributes to explore, we also created the following features out of the data for our analysis:

Name and blurb (description) length including and excluding “stop words” - name_len_clean, blurb_len_clean
Day of week and hour of the day for creation, launch and deadline date - deadline_weekday, created_at_weekday, lauched_at_weekday, deadline_hour, created_at_hour, launched_at_hour
Days between creation and launch, and days between launch and deadline - create_to_launch, launch_to_deadline




each project has 15 features:

1. **ID** : project ID.
2. **name** : the name of the project.
3. **main_category** : the main category the project.
4. **category** : a subgroup of main_category.
5. **currency** : the currency of the project.
6. **deadline** : the deadline of the project.
7. **goal** : goal amount in project currency.
8. **launched** : the launch date for the project.
9. **pledged** : pledged amount in the project currency.
10. **state** : state is a categorical status of the project.
11. **usd pledged** : pledged amount in USD (conversion made by KS).
12. **usd_pledged_real** : pledged amount in USD (conversion made by fixer.io).
13. **usd_goal_real** : amount of USD the project asked for initially.
14. **backers** : the number of supporters that actually invested in the project.
15. **country** : country of origin of the project.


in this project, we can find out :

- what is the most common category of kickstarter projects.
- what is the average amount of pledged(USD), goal and backers.
- what is the accuracy score of the prediction model.
- what is the most important factor in having successful project.

i will use the must-have python packages for Data Science and Finance:
- NumPy : Allowing us to work with multidimensional arrays, and a fast numeric array computations
- Pandas : Allowing us to organize data in a tabular form, and quickly loading remote data or a .csv file.
- Sklearn : Machine Learning in Python, Simple and efficient tools for data mining and data analysis.
- Matplotlib : is a Python 2D plotting library.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites
 - Docker
 
 ### Installing
 
 1. Copy the project to your machine
 
     ```
     git clone https://github.com/ayoubabozer/kickstarter.git
     ```
 
 2. Get into the Dir
    
    ```
    cd kickstarter
     ``` 
 
 3. Pull & Run Docker Image
 
     ```
     docker run -d --rm --name jupyter -p 8888:8888 -v $PWD:/opt playniuniu/jupyter-pandas
     ```
 4. Open the app in : [http://localhost:8888](http://localhost:8888)


# ENJOY!.
