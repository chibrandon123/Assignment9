# Web Scraper Notebook
## General functionality of Web Scraper
- This notebook contains functionality to grab html code from the specified url "https://corgis-edu.github.io/corgis/csv/". 
- To grab the html code, the notebook utilizes the 'requests' python library and converts into a readable text string.
- Utilizing the 'BeautifulSoup' library, we create an html parser object that we can utilize to query specific html tags for search.
- We have a function grabDataDF(name) which takes in the name (of type string) of the dataset we want from the above url. This function does a series of parsing in which it appends the given name of the dataset to the url, downloads the corresponding csv by finding the <a/> html tag with the 'href' attribute to get the link, and reads it into a dataframe using the 'pandas' library.
## Billionaires Dataset
- After the data is grabbed and stored in a workable data structure, some analysis is done in which it finds the top 20 ranked billionaires and displays there name sorted by rank.
- Plot type: Bar Chart
## Drugs Dataset
- The same process is repeated for a different dataset labeled "Drugs". 
- The analysis done on this dataset is a bit different: we filter the data to only include the data pertaining to the state of California.
- It then plots the prevlance of alcohol use disorder over time for California.
- Plot type: Line Graph
## Health Dataset
- Finally, we do the same thing with the dataset labeled 'Health'. 
- We filter the data to only include lines pertaining to the 'Measles' virus and plots the frequency of measles outbreaks over the years. 
- Plot type: Histogram

