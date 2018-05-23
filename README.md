# Althawk
Althawk is a social-minded cryptocurrency analysis project. First, both fundamental and technical data specific to certain 'alt' coins is harvested and stored in a database. Various natural language processing and machine learning techniques are then applied to the aggregated data to gather insights and/or predictions. The result will be deployed and presented to the end-user.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What libraries, packages you need to have installed:

```
Python
Sqlite
Pandas
Datetime
Requests
Jupyter notebook
```

## Running the tests

- Simply run Gatherer.py to start fetching data and saving this to a sqlite database.
- Run Worker.py to gather data

## Continuity

- Add #!/usr/bin/python3 to top of code & don't forget to chmod a+x Worker.py
- Add this line to sudo crontab -e to run hourly: 5 */1 * * * cd /home/althawk/Althawk && ./Worker.py > /home/althawk/Althawk/cronlog.log 2>&1

## Built With

* [Cryptocompare](https://min-api.cryptocompare.com/) - The API used to gather historical data
* [Twitter](https://developer.twitter.com/en/docs) - Twitter API for scraping tweets

## Authors

* **Boaz Vetter** - *Founder* - [x3r4](https://github.com/x3r4)
