# Scrapelo

This simple package provides functions for obtaining ELO scores for clubs available on [clubelo.com](http://clubelo.com/). <br>
If You wonder how does the ELO system work, You can read about it [here](http://clubelo.com/System).

## Installation
```
pip install scrapelo
```
<br>

## Features

### Get the current ELO scores of clubs for a given competition.
```
import scrapelo
scrapelo.get_competition_elo('Champions League')
```
![](https://raw.githubusercontent.com/AKapich/Scrapelo/main/ucl_table.png?token=GHSAT0AAAAAACONR7OMWQNWGEJBZBMLMR5GZPETJXA)

The same effect can be achieved by using the competition code instead of the competition name. You can find out the full list of codes [here](https://github.com/AKapich/Scrapelo/blob/main/country_codes.py).
```
import scrapelo
scrapelo.get_competition_elo('UCL')
```

For the country competitions the argument ought to be the country's name in English or the country's code. 
```
import scrapelo
# two lines below will give You the same output
scrapelo.get_competition_elo('Spain')
scrapelo.get_competition_elo('ESP')
```
### Get the current ELO of a single club.
```
import scrapelo
# Function takes only club name as an argument 
scrapelo.get_club_elo('Barcelona')
```
<br>

## Legal Scraping

The data is scraped legally, as the [robots.txt](http://clubelo.com/robots.txt) file on the website allows for it.
