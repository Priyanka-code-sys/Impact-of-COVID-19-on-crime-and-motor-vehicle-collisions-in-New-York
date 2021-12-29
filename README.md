# Database_and_Analytics_Programming

DAP_L Project
Karan veer singh  x20146248
Priyanka          x20192037
Murugappan        x19239831

PLEASE DOWNLOAD ALL THE FILES AS A FEW VISUALIZATIONS ARE DONE IN PLOTLY AND MIGHT NOT RENDER WELL IN GITHUB

x19239831_Motor_Vehicle_Collisions.ipynb
Priyanka-Covid-19-deaths.ipynb
x20146248_Karan.ipynb
Combined_Visualizations(2).ipynb

We tried to implement the SSH tunneling and done with coding as well and created user for you as well but we are not sure that can be tested from your end and so we dont want to make it risk at the end and so we had not implemented the tunneling. So, We team members requesting you to setup the cloud server in your local mongodb and postgres db using the credentials inputed in all of our individual files. Below is the Attached file for the code created for SSH tunneling for your reference

ssh_Connect_Using_pem_key.ipynb
ssh_connect_from_local.ipynb

We have also converted data fetched from the API into a csv format for your reference, just in case you need it (Attached the Zip File)

Datasets_csv.zip

Please run the master Jupyter Notebooks (Run the attached individual Jupyter Notebooks):
Combined Automated File for Group-L.ipynb

Dataset1: Provisional COVID-19 Death Counts by Sex, Age, and State
Dataset URL: https://data.cdc.gov/NCHS/Provisional-COVID-19-Death-Counts-by-Sex-Age-and-S/9bhg-hcku

Dataset2: Crime Incidents
Dataset URL: https://data.buffalony.gov/Public-Safety/Crime-Incidents/d6g9-xbgu

Dataset3: Motor Vehicle Collisions - Vehicles
Dataset URL: https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Vehicles/bm4k-52h4

Attached the requirements file for the project
requirements.txt

The research idea is to determine the impact of covid over the crime and vehicle crashes in New York State. 

# Methodology

 This research consists of 3 distinct datasets which is about Covid, Crime and Vehicle Collisions. These three are all API's. By hitting the API everytime, we are getting the real time records. 
Here, our project process is to take the raw json through API and push it into MongoDB. Retrieving the JSON from mongo and doing the data preprocessing and transformation like renaming columns, dropping irrelevant columns and na values, filtering rows based on certain conditions, replacing columns values, date formatting.
Then finally pushed the structured data to postgres DB by creating tables. creating joins using sql to get combined dataframe to perform visualizations and to give useful insights.
The project is hosted in microsoft azure cloud server with linux based debian distribution virtual machine installed for integrating all the team members works. so, enabled the fire wall using linux command in server and tried to tunnel through the SSH port for additional security purpose. In server, Installed both the Mongo and postgres DB. The specifications of the server is 1GB RAM size and 30GB memory with 1 CPU. Through SecureSHell PuTTY connecting to server using azureuser. Installed ROBO3T mongo client and Pg Admin 4 postgres client to access the server.

# Objective and Outcome of the project
The objective of this research is to show how the covid impacted the crimes and motor vehicle collisions in New York City in United States.

The combined outcome of this research is that accidents got decreased because of lockdown imposed all over the state and crimes got increased because of covid unemployment and multiple factors.


# Files

Following the uploaded files
1) Each individual data cleaning file
2) Combined Visualization file
3) Master Notebook for automation
4) Each data files
5) Backup file

## Libraries Used
import urllib.request as request
import json
import pymongo
from pymongo import MongoClient
import urllib.parse
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
import psycopg2

Thanks to matplotlib, seaborn , plotly for providing resources for our projects to do visualizations




