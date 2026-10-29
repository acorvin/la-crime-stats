# LA Crime Analysis 2020-2023 

A Python project exploring Los Angeles crime data from 2020 to 2023. The goal is to find crime trends, patterns, and hotspots using data exploration and visualization.

### Dataset

The dataset used for this analysis can be downloaded here **[Data.gov](https://catalog.data.gov/dataset/crime-data-from-2020-to-present)**

The version used here has 798,242 reported crimes and 28 columns, including the date and time of each crime, the LAPD area, the crime type, victim details, the premises, the weapon used, and latitude/longitude. It contains no duplicate rows.

The CSV isn't included in this repo because of its size. To run the notebook, download it and save it as `data/la-crime-data.csv`.

### Questions explored

All of the analysis is in [`la-crime-stats.ipynb`](la-crime-stats.ipynb).

**What are the most common crimes?**

| Crime | Share of all reports |
|---|---|
| Vehicle stolen | 10.7% |
| Battery, simple assault | 7.9% |
| Theft of identity | 6.4% |
| Burglary from vehicle | 6.1% |
| Vandalism, felony ($400 and over) | 6.1% |
| Burglary | 6.1% |
| Assault with a deadly weapon, aggravated assault | 5.8% |
| Petty theft ($950 and under) | 5.1% |
| Intimate partner, simple assault | 5.0% |
| Petty theft from a motor vehicle ($950 and under) | 3.9% |

**What are the least common crimes?** The rarest offense types each appear only a handful of times. Inciting a riot appears once, and dishonest employee attempted theft appears twice.

**Which year had the most crimes?**

| Year | Reported crimes |
|---|---|
| 2020 | 199,365 |
| 2021 | 209,288 |
| 2022 | 234,060 |
| 2023 | 155,529 |

Reports rose each year from 2020 to 2022. The 2023 figure covers only part of the year, so it can't be compared directly with the others.

**Which areas saw the most crimes?** A bar chart compares total reports across LAPD's 21 areas.

**Which months had the most crimes?** A heatmap shows reports for every month of every year.

### How to run

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook la-crime-stats.ipynb
```

The notebook reads the file with the `iso8859_11` encoding.

### Technologies

**[Python](https://www.python.org/)**

**[pandas](https://pandas.pydata.org/)**

**[Matplotlib](https://matplotlib.org/)**

**[Seaborn](https://seaborn.pydata.org/)**
