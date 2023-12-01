---
title: Data and Methods
summary: Summary
date: "2018-06-28T00:00:00Z"
editable: true
share: false
---
## Faculty Data

Data for USC Price faculty will be gathered from the [Price faculty page](https://priceschool.usc.edu/faculty/)  
We can obtain name, contact, position, expertise, degrees, and a biological sketch of each professor.  

## Google Scholar Pages

Most faculty have a Google Scholar Page, where we can pull data relating to each faculty's research publications.
Each publication has a title, authors, year, and number of citations, as well as a vast pool of textual data.

## Extraction Methods

Using Python with Google Colab notebooks, we generated a web-scraping script that obtained the necessary information. 
Package BeautifulSoup provided a framework for obtaining data from each webpage.  

"Information for faculty and their publications were stored in dictionaries as key:value pairs and connected by faculty name as the primary key."

Extracting data from the text of publications proved to be a difficult task, one we did not complete during the scope of this semester. 

Using spaCy, we were able to generate named entity recognitions and successfully fetch the dataset names using custom rules of finding organizations (example: JULIET clinical trial).  
However, the variation among the format of publications yielded poor model training results.  
