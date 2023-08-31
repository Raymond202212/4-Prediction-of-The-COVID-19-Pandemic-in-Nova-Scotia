<!--- The following README.md sample file was adapted from https://gist.github.com/PurpleBooth/109311bb0361f32d87a2#file-readme-template-md by Gabriella Mosquera for academic use ---> 
<!--- You may delete any comments in this sample README.md file. If needing to use as a .txt file then simply delete all comments, edit as needed, and save as a README.txt file --->

# 4. Prediction of The COVID 19 Pandemic in Nova Scotia

**[Abstract]** COVID-19 is a pandemic that has once outbroken worldwide. Such a pandemic significantly effected Nova Scotians' Health and cast a series of social impacts in our Healthcare Domain. This project would use the Auto-Regressive (AR) Model and the Auto-Regressive Integrated Moving Average (ARIMA) to predict the pandemic in Nova Scotia from June 2023 to August 2023, based on the data provided by <a>https://health-infobase.canada.ca/covid-19/</a>.

* *Date Created*: 30 August 2023
* *Last Modification Date*: 31 September 2023

## Authors

* [Raymond Liu](mailto:Raymond.Liu@dal.ca)

## Getting Started

### Prerequisites

To have a local copy of this lab, you can use either google colab or jupyterlab to execute the `code.ipynb` file. You shall execute the code block in order.

## Sources Used

<!--If in completing your lab / assignment / project you used any interpretation of someone else's code, then provide a list of where the code was implement, how it was implemented, why it was implemented, and how it was modified. See the sections below for more details.-->

### `CODE.ipynb`

*Chapter 0 2nd block*

```
url = "https://health-infobase.canada.ca/src/data/covidLive/covid19-download.csv"
s=requests.get(url).content
df = pd.read_csv(io.StringIO(s.decode('utf-8')))

```

The code above was created by adapting the code in [stackoverflow](https://stackoverflow.com/questions/32400867/pandas-read-csv-from-url) as shown below: 

```
import pandas as pd
import io
import requests
url="https://raw.githubusercontent.com/cs109/2014_data/master/countries.csv"
s=requests.get(url).content
c=pd.read_csv(io.StringIO(s.decode('utf-8')))
```

- <!---How---> The code in <a href = 'https://stackoverflow.com/questions/32400867/pandas-read-csv-from-url'>stackoverflow</a> was implemented by smci.
- <!---Why---> <a href = 'https://stackoverflow.com/questions/32400867/pandas-read-csv-from-url'>stackoverflow</a>'s Code was used to access the corresponding data resource directly from the given link.
- <!---How---> <a href = 'https://stackoverflow.com/questions/32400867/pandas-read-csv-from-url'>stackoverflow</a>'s Code was directly used by the author.



## Acknowledgments

* I am thankful to Professor Thomas Trappenberg on tutoring the course, *Fundamentals of Machine Learning (CSCI 6505)*, and to the bootcamp on tutoring the project framework and the usage of the corresponding models.
* The implementation of the project is only for educational purpose, and the corresponding result is only for reference.
