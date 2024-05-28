# IBM-DataScience

## Project background
Project background was to explore SpaceX data of rocket launches. From the data I was to clean, process, and predict best parameters which will affect success rate of the launches.
Question here was which parameters would clearly affect on success of the launch. In many processes the parameters examined were related the Flight Number, Launch Site, Payload Mass or Orbit type targeted.
Lastly it was to predict with different machine learning models how the landing would end up, and find best performing model.

## Methodology
Data collection methodology included using Python’s libraries for API requests, Numpy, Pandas and Datetime. Performing GET request and have the data return as JSON. From there to filter and collect information that was later used for our predictions. These would include rocket booster name, payload mass and orbit, launchpad and its location, outcome, type of landing, number of flights and few more. Data wrangling would include filtering data, replace NaN values with mean method. 
Some data was collected via webscraping the Wikipedia page of Falcon 9 and Falcon Heavy launches. In this information was collected with Python as well, performing GET requests, creating beautiful soup object, parse HTM, extract names from table headers, create empty dictionaries from keys of extracted column names, parse them, fill a dictionary, and convert into a data frame.
Also external CSV file was used, transferred to database and performed data collection with Python as well as SQL queries with the help of SQL Alchemy.
The data was then visualized with Python’s visualization libraries such as Matplotlib and Seaborn, and with interactive methods such as Plotly and Dash.
In the last part, machine learning techniques were used to create models that best predict these changing variables. Method of Decision Trees, K-Nearest Neighbours and SVM were used.




