# Scoresaber Leaderboard scraper

A basic html scraping script that scrapes the scoresaber leaderboards page for player rank, pp and country of origin.

By default the script will scrape the first 2000 pages (equivalent to the top 100k beat saber players) of [https://scoresaber.com/global](https://scoresaber.com/global) to produce a csv file named: `leaderboard-rankings-DD-MM-YYYY.csv` 

Formatted similarly to the following:

| Rank | Player | PP | Country  |
| ---- | --- | --- | --- |
| 1 | Tammymatty | 4874.11 | United States |
| 2 | TTV RogdudeVR | 4682.16 | Sweden | 
| 3 | OrangeW | 4665.77 | United Kingdom |

Takes about an hour to run (2 seconds per page).

### Requirements
 * Python 3.0+
 * Requests Library (`python pip install requests`)

### Usage

Open cmd prompt and run:
```
python scoresaber-scraper.py
```

### Optionl Variables

You can optionally set the values `startpage` and `endpage` inside `scoresaber-scraper.py` to change the page on which scraping starts and ends.