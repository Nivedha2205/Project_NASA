                                        🚀 NASA Near-Earth Object (NEO) Tracking & Insights using Public API

             NASA Near-Earth Object (NEO) Tracking & Insights using Public API is an data science project created to collect datas directly from NASA's server using unique API key provided by NASA. The data set contains all the information from date to date regarding the asteriods that nearer the earth. 
             So from the raw datas collected we can get the required data using Python code and create an database using SQL code and converting the required data into an dashboard using Streamlit code.

PROJECT'S DOMAIN:
            Space Research & Astronomical Data Analysis

SKILLS DEVELOPED FROM THIS PROJECT:
             1. API Integration and JSON Parsing
             2. Data Transformation 
             3. Relational Database (SQL) Table Creation and Insertion
             4. Query Writing for Analytical Insights
             5. Streamlit Dashboard Development
             6. Filter-Based Data Interaction

STEP BY STEP APPROACH:

    STEP1: 
    1. Getting the NASA API Key
    
    2. Go to: https://api.nasa.gov

    3. Fill in your name and email, and submit the form to register.

    4. Your API key will be sent to your email address.

    5. The key will look like “qSxX9kz1L7....”

    6. Use your key to format the API URL.

    STEP2: Extract Data Using NASA's Asteroid API

    1. Beginning with a start date (2024-01-01) and an end date 7 days later (2024-01-07).
    
    2. Using Pagination via the 'next' Link.

    3. After processing the first response, getting the 'next' URL from data['links']['next'].

    4. This link points to the next 7-day date range.

    5. Updating the request URL and repeat the process.
    
    6. Repeating Until 10,000 Records Are Collected.
    
    7. Keep looping through the 'next' links.
    
    8. Each response brings data for 7 days.
    
    9. Append extracted fields into a list.
    
    10. Stopping when the list reaches 10,000 asteroid records.

  STEP 3: DATA CLEANING

    1. Extracting the required fields as given below by using JSON response.

    The required fields are id,neo reference id, name, absolute magnitude h, estimated diameter min km, estimated diameter max km,
    is potentially hazardous asteroid, close approach date, relative velocity kmph, astronomical, miss distance km, miss distance lunar and 
    orbiting body.

    2. Converting the data into the correct format of data types to int,float,date from string.

    3. Now ensuring the formatted data types for the SQL Insertion. 

  STEP 4: Inserting the NASA's Asteroid Data into SQL.

    1. Creating an database by using My SQL workbench.

    2. Creating an connection for python and SQL by using mysql.connector.

    3. Creating an cursor object.

    4. Two tables - Asteriods and Close approach data have been created as per the requirement.

    5. Now using insert queries to feed the created table.

  STEP 5: REAL TIME SQL QUERIES OF 15+ QUERIES HAVE BEEN CREATED.

    1. 15+ queries have been created using sql code.

    2. These queries will be displayed in the streamlit dashboard.

  STEP 6: CREATING STREAMLIT DASHBOARD 

    1. Creating streamlit dashboard to filter datas with options like
                sidebar ,
                slider,
                dropdown,
                date pickers,etc.

    2. Now the fully functional dashboard will be created by running the streamlit file in python.


CONCLUSION OF THIS PROJECT:

    1. NASA'S API KEY has been extracted from the nasa's server.

    2. The URL repeating process will be stopped once the collected data reaches the count of 10000.

    3. The collected raw will be cleaned and formatted for the SQL insertion.

    4. Two tables have been created and datas heen inserted using the required code.

    5. For an real time experience, an STREAMLIT dashboard has been created.           


        

             


