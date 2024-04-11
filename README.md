# geeksrter_simoesh_kindo

import requests
from bs4 import BeautifulSoup

# URL for scraping data
url = 'https://data.covid19india.org/v4/min/timeseries.min.json'
page = requests.get(url)
print(page)
soup= BeautifulSoup(page.content, 'html.parser')
print(soup)
