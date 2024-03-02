Greetings and welcome to the comprehensive documentation on real-time stock analysis facilitated by the seamless integration of Copilot and Microsoft Fabric. This guide presents user-friendly and efficient methods for visualizing market data in the most convenient manner.



Objective:

In the contemporary landscape, streaming data has emerged as a pivotal element in various domains. Numerous operations necessitate real-time data analysis, with stocks and market data standing out as prime examples of such streaming data. This documentation elucidates the profound impact of leveraging the services of Fabric and Copilot to effectively utilize real-time stock data for in-depth analysis and the creation of visually compelling reports.


1. Setting up notebook for Streaming data retrival and making it ready for analysis
Step 1: proceed with the installation and importation of requisite libraries

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/b214dd23-19af-489f-9e9e-5b1326fac5cf)

We employ the libraries Requests and BeautifulSoup for web scraping purposes. These libraries enable the retrieval of data through APIs of multiple URLs and facilitate parsing of responses to extract the necessary information.

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/ecf6d591-6488-4f87-951c-49739d96f7db)


Step 2: Using pandas dataframe to load the data into desired format. Changing Columns as per requirements.

Step 3: Loading Data into Microsoft Fabric LakeHouse

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/d17ca8c8-bb33-4708-9605-24cb6d5afea2)

Step 4: Reading the LakeHouse file into spark dataframe and changing columns as per requirements then converting it into Delta table

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/76e2438d-2003-48ab-9886-e62beb2acae3)

Now, the notebook is ready for the job.




2. Setting up data pipeline in MS Fabric to get real time data through schedule run of the pipeline.

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/40e79309-a5ac-46bb-a33d-1c9028dcaa4c)



3. This will provide us with data in delta table with timestamp, which can be used for analysis and visualization, with custom charts and useful details with real time refresh. 

![image](https://github.com/Kapamania/Fabric_Hackathon_2024/assets/17914333/7f45605f-2930-43b4-b17e-1a09acc85a3e)








