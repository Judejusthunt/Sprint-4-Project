# Sprint-4-Project
This is the Repository that will be used for my Sprint 4 Project in the Triple Ten Data Science Program.


# Project Description :

The focus of this project is to provide you with additional practice with common software engineering tasks. These will augment and complement your data skills, and make you a more attractive job candidate to potential employers.
The tasks are: creating and managing python virtual environments, developing a web application, and deploying it to a cloud service that will make it accessible to the public.
In this project, we are providing you with a dataset you are already familiar with: a dataset of car sales advertisements. However, in this project, the focus will not be on the dataset or the analysis, and thus you are free, and even encouraged, to choose any dataset that you want.
The project is split into several steps that replicate the process described in one of our blog posts.

Demo of the web application you’ll build in this project
Instructions for completing the project
Step 1. Project Prerequisites
Create an account on github.com
Create a new git repository with a README.md file and a .gitignore file (choose a Python template).
Install at least the following packages: pandas, streamlit, plotly-express. Feel free to install more packages if you want to implement additional features in your web app.
Create an account on render.com, link it to your GitHub account
Install VS Code, load the project directory and set the Python interpreter to the one used by the virtual environment
Step 2. Download the data file
Download the car advertisement dataset (vehicles_us.csv) or find your own dataset in a CSV format
Place the dataset in the root directory of the project
Note: for project ideas and inspiration, check out this video.
Step 3. Exploratory Data Analysis
Create an EDA.ipynb Jupyter notebook in VS Code
Save the notebook in the notebooks directory of your project
Perform some basic exploratory analysis of the dataset in the notebook
Create a couple of histograms and scatterplots using plotly-express library
Note:
if you are using the car advertisement dataset, it won’t be sufficient to simply recreate the plots described in the blog post to complete the project. You’ll have to get creative and come up with your own plots and histograms.
it’s often very convenient to experiment with data visualizations in Jupyter, and then copy-paste code into a web application file later
Step 4. Develop the web application dashboard
Create an app.py file in the root of the project’s directory
Import streamlit, pandas and plotly_express
Read the dataset’s CSV file into a DataFrame
Create and/or copy from the Jupyter notebook:
at least one st.header with text
at least one plotly-express histogram using st.write or st.plotly_chart
at least one plotly-express scatter plot using st.write or st.plotly_chart
at least one checkbox using st.checkbox that changes the behavior of any of the above components
Don’t forget to update the README file when you are done. It should contain some basic description of the project and instructions on how other people could launch your project on their local machine if they wanted to.
IMPORTANT: Replit will fail to build your project unless all project files are present in your GitHub repository. Therefore, you must commit and push file changes to your repository when you’re done with your work.
Notes:
as you develop your application by adding a new Streamlit component, you can run streamlit run app.py command from the terminal to see what the result looks like
as you reach some milestones in the application development (e.g. you add a working component and the application runs without errors), it’s a good practice to commit and push your work to a remote repository on GitHub. So don’t forget to write a meaningful commit message!
Step 5. Deploy the final version of the application to Render
To make streamlit compatible with render, add a streamlit configuration file to your git repository at .streamlit/config.toml with the following content:
[server]
headless = true
port = 10000

[browser]
serverAddress = "0.0.0.0"
serverPort = 10000 
It’ll tell Render to look in the right place to listen to your streamlit app when hosting it on its servers.
Open your account on render.com and create a new web service:

image
Create a new web service linked to your Github repository:

image
Configure the new Render web service. To your Build Command, add
pip install streamlit & pip install -r requirements.txt 
To your Start Command, add: streamlit run app.py. It should look like this:

image
Deploy to Render, wait for the build to succeed:

image
Verify that your application is accessible at the following URL: https://<APP_NAME>.onrender.com/
Note: it can take several minutes after a succesful deployment for the app to be available online on a free tier. Also note that apps go “asleep” after being inactive for a few minutes. If so, just load and refresh your app a few times for it to get awoken.
How to submit my project:
You’ll need to submit a link to your GitHub repository. Please also add the URL of your app on Render to your project’s README.md
How will my project be evaluated?
We've put together some project assessment criteria. Read over them carefully before you make a submission.
Here’s what project reviewers look for when assessing your project:
Does the project repository contain at least the following files?

# The minimal expected project structure
$ tree
.
├── README.md
├── app.py
├── <name_of_your_dataset>.csv
└── notebooks
    └── EDA.ipynb
└── .streamlit
    └── config.toml 
Is the web app accessible via a browser?
Does the web app contain the following?
at least one header with text
at least 1 histogram
at least 1 scatter plot
