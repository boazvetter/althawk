# Althawk
Althawk is a sentiment-aware cryptocurrency social analysis project. First, both fundamental and technical data specific to certain 'alt' coins is harvested and stored in a database. Various natural language processing and machine learning techniques are then applied to the aggregated data to gather insights and/or predictions. The result will be deployed and presented to the end-user.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Libraries, packages you need to have installed:

```
Python
Sqlite
Pandas
Datetime
vaderSentiment
```

## Running the tests

- (Optional) Run Gatherer.py to start fetching data and saving this to a sqlite database.
- Run Worker.py to gather data

## Continuity

- Add #!/usr/bin/python3 to top of code & don't forget to chmod a+x Worker.py
- Add a line to sudo crontab -e to run periodically, for example 5 minutes past every hour: 5 */1 * * * cd /home/althawk/Althawk && ./Worker.py > /home/althawk/Althawk/cronlog.log 2>&1

## Built With

* [Cryptocompare](https://min-api.cryptocompare.com/) - API used to gather historical price data
* [Twitter](https://developer.twitter.com/en/docs) - Twitter API for scraping tweets
* [Vader](https://github.com/cjhutto/vaderSentiment/) - Lexical sentiment analysis tool

## Authors

* **Boaz Vetter** - *Founder* - [x3r4](https://github.com/x3r4)
