# ECE143_Project - San Diego police calls for service Analysis

The dataset source is from: https://data.sandiego.gov/datasets/police-calls-for-service/

This project aims to analyze the dataset of police calls for service dispatched by the San Diego Police
Department’s communications dispatch center. A police call service dataset can provide valuable insights into
various aspects of public safety, law enforcement, and community well-being. The dataset contains various
attributes such as incident number, date/time, day of the week, location details, call type, disposition, beat,
and priority. This enriched dataset can allow us to explore a variety of patterns behind police call service.
By analyzing this dataset, we aim to identify hotspots for different types of incidents, peak times for calls,
and potentially uncover any patterns related to specific call types or areas.

Additional Notes: We used the data from 2019 to 2023, which is huge and cannot be uploaded to repo. You can find detailed information about data from [Dataset information](#jump). 

## <span id="jump">Dataset inforamtion</span>

![Image Alt Text](https://github.com/rayxuan2000/UCSD_ECE143_project/blob/e7b49164afbe4e7959522b9ca60591bfedec7cb6/additional/data_frame.png)
## File Structure of ECE143_Project.ipynb
### Part 0: Initializations and packages import
#### Initialization
Install pydrive to load data stored in the Google Drive.

#### Package import
Import all the package in [Modules](#jump).

### Part 1: Data collection and cleaning
#### Prepossessing
Store data file id in the dictionary.
#### File extraction
Extract all files based on file id and concatenate data as dataframe from 2019 to 2023.
#### Cleaning functions
Write functions to do data cleaning such as empty removal, date_time seperation, weekday conversion, etc. 
#### Data cleaning
Apply above functions to data.

### Part 2: Exploratory data analysis and visualization
* Analysis 1: Call based on year
* Analysis 2: Call based on month
* Analysis 3: Call based on days in a week (Monday, Tuesday...)
* Analysis 4: Call based on hours (1AM-2AM, 2AM-3AM...)
* Analysis 5: Call type and priority
* Analysis 6: Disposition
* Analysis pro: Map visualization
For Map visualization part, if you could not preview it in ECE143_Project.ipynb, then click this HTML file [Open HTML file in new window](additional/map_with_legend.html){:target="_blank"} and see it in a new window.

## How to run the code
Our project is based on google colab platform. Just open ECE143_Project.ipynb as a jupyter notebook file and run each cell.

##   <span id="jump">Modules</span>
* numpy 
* pandas
* math
* matplotlib.pyplot
* calendar
* seaborn
* folium
* IPython.display.display
* geopy.geocoders.Nominatim
* time
* collections.Counter
