# Quality of Life vs Cost of Living

I want to know **which cities in the world offer a good bang for your buck**, that is, cities that are relatively cheap and with a high quality of life. 

Therefore, I'll be comparing the quality of life and the cost of living for cities around the world. 



## Data

I'll be using data from the website [Numbeo](https://www.numbeo.com/cost-of-living/). They have two indexes:

* [Quality of Life Index 2024](https://www.numbeo.com/quality-of-life/rankings.jsp), by city
* [Cost of Living Index](https://www.numbeo.com/cost-of-living/rankings.jsp), by city



###  Ingestion

Since the dataset is not too large, I will simply copy and paste the data into a spreadsheet in Google Sheets.

| Index                        | File                                                         | Date accessed | Number of rows |
| ---------------------------- | ------------------------------------------------------------ | ------------- | -------------- |
| Quality of Life Index (2024) | [Spreadsheet](https://docs.google.com/spreadsheets/d/1DhfMyU7d0Bxpt5o1_Z3fuSz3ThjcGFBFzS1Yi59osuY/edit?usp=sharing) | 01 Jul 2024   | 178            |
| Cost of Living Index (2024)  | [Spreadsheet](https://docs.google.com/spreadsheets/d/1DhfMyU7d0Bxpt5o1_Z3fuSz3ThjcGFBFzS1Yi59osuY/edit?usp=sharing) | 01 Jul 2024   | 370            |

The Quality of Life Index dataset already includes cost of living as a column. Therefore, I can continue with my analysis only using this dataset. I'll download a local copy to my computer.

However, I noticed that the Cost of Living Index includes additional fields (as well as more cities). I'll keep this dataset in case I need it for future analyses.



### Cleaning

I notices that, in the Quality of Life dataset, the *City* column includes for city and country. For US cities, it also includes the state. I'll split the field to have city and country in different columns.

To automate the process for future analyses, I'll do the cleaning in Python.

 







