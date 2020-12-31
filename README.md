# NHL

The purpose of this project is to:

1. demonstrate web scraping via Python's Beautiful Soup module
2. demonstrate Python-MySQL connectivity
3. demonstrate data exploration using Python/SQL interactions

Towards this end we have chosen an NHL data set, scraped from [hockey-reference.com](http://hockey-reference.com)

## Files

- scrape.ipynb: scrapes [hockey-reference.com](http://hockey-reference.com) for NHL data, storing it in a MySQL database
- leaders.ipynb: looks at historical NHL scoring leaders, normalizing player stats for league-wide scoring 
- draft.ipynb: looks at the offensive output of NHL players compared to their draft status
- countries.ipynb: looks at the NHL makeup by nationality over time

## Prerequisites

- python3
- jupyter
- the following Python modules: scipy, numpy, pandas, requests, bs4, lxml, sqlalchemy, mysql-connector-python, html5lib
- MySQL: [install](https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/) and create a new database and user
```
CREATE DATABASE nhl;
CREATE USER 'nhl'@'localhost' IDENTIFIED BY 'hockey';
GRANT ALL PRIVILEGES ON nhl . * TO 'nhl'@'localhost';
```
