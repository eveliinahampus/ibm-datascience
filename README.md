# IBM Data Science Project

## Project Background

The project's objective was to explore SpaceX rocket launch data. From this data, I was tasked with cleaning, processing, and predicting the key parameters that influence the success rate of launches. The main question was which parameters clearly affect the success of a launch. Several factors were examined, such as flight number, launch site, payload mass, and the type of orbit targeted. Lastly, the focus was on predicting landing outcomes using different machine learning models to identify the best-performing model.

---

## Methodology

The data collection process involved using Python libraries such as `requests`, `NumPy`, `Pandas`, and `datetime`. Data was fetched via API requests and returned in JSON format. This was filtered to extract key information like the rocket booster name, payload mass, orbit type, launch pad location, outcome, landing type, and flight numbers, which were later used for predictions. Some of the data was collected by web scraping the Wikipedia page of Falcon 9 and Falcon Heavy launches using Python. This involved performing `GET` requests, creating BeautifulSoup objects to parse HTML, extracting table headers, building dictionaries, and converting them into a structured DataFrame. 

An external CSV file was also used, transferred into a database, and further processed using SQL queries and Python with the help of SQLAlchemy. Data wrangling included filtering the data and replacing NaN values with the mean method to clean and reorganise the information for analysis. The processed data was then visualised using Python's visualisation libraries. Static visualisations were created with Matplotlib and Seaborn, while interactive visualisations were developed with Plotly and Dash.

In the final stage, machine learning techniques were used to predict the outcomes of launches. Models such as Decision Trees, K-Nearest Neighbours, and Support Vector Machines were applied to identify the best-performing method for predicting landing outcomes.

---
```
### Data Collection  
The data was collected using Python libraries such as `requests`, `NumPy`, `Pandas`, and `datetime`.  
- Data was fetched via **API requests**, with results returned in JSON format.  
- Key parameters like the rocket booster name, payload mass, orbit type, launch pad location, outcome, landing type, and flight numbers were filtered and stored for analysis.

Additionally:  
- Web scraping was employed to gather data from the **Wikipedia page for Falcon 9 and Falcon Heavy launches**. Using Python, this involved:
  - Performing `GET` requests.
  - Creating BeautifulSoup objects to parse HTML.
  - Extracting table headers and constructing dictionaries.
  - Filling the data into a structured DataFrame.

An **external CSV file** was also used. This data was imported into a database, where **SQL queries** (with `SQLAlchemy`) and Python were utilised for further processing.

### Data Wrangling  
- Filtering data and replacing `NaN` values using the mean method.  
- Cleaning and reorganising the data for analysis.

### Data Visualisation  
The data was visualised using Python libraries:
- **Static methods**: `Matplotlib`, `Seaborn`.
- **Interactive methods**: `Plotly`, `Dash`.

### Machine Learning  
To predict outcomes, various machine learning techniques were applied, including:
- **Decision Trees**  
- **K-Nearest Neighbours (KNN)**  
- **Support Vector Machines (SVM)**  

The models were evaluated to determine the best-performing approach for predicting landing outcomes.
```
---





