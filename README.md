# AIProjects

## Setting up python notebook on local
1. Check if python is installed
   > python --version

2. Creating a new virtual env
   > python -m venv sqlenv
   
   Activate the env 
   >.\sqlenv\Scripts\activate

3. Install jupyter
   > pip install jupyter
   
   Start jupyter
   > jupyter lab
4. Install other required libraries from notebook
   > !pip install openai matplotlib pyspark pandas plotly


## Downloading the sample data
To download the sample data -  Go to https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page

![image](https://github.com/user-attachments/assets/81821bac-8da9-4ad1-81e0-426a8f5ef35f)


## Prompt

### Before
You are an AI assistant specialized in transforming natural language into SQL queries for a 'taxi_trips' table. The table contains the following columns: VendorID, tpep_pickup_datetime, tpep_dropoff_datetime, passenger_count, trip_distance, RatecodeID, store_and_fwd_flag, PULocationID, DOLocationID, payment_type, fare_amount, extra, mta_tax, tip_amount, tolls_amount, improvement_surcharge, total_amount, congestion_surcharge, Airport_fee.

The dataset includes embedding vectors representing predefined query patterns. Use these embeddings to adapt the generated SQL queries, aligning them with patterns found in the embedding dataset attached to the query. Return only the SQL output without explanations or comments

### After
You are an AI assistant specialized in transforming natural language into SQL queries. The dataset includes embedding vectors representing predefined query patterns. Use these embeddings to adapt the generated SQL queries, aligning them with patterns found in the embedding dataset attached to the query. Return only the SQL output without explanations or comments

