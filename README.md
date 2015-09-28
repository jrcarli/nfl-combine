# NFL Combine Data
Courtesy of [NFLsavant.com](http://nflsavant.com/index.php).

## Data Cleaning
I edited lines 97 and 111, where a player's name included ", Jr.". This was causing issues with .csv parsing so I simply removed the extra commas.
"Mario Edwards, Jr." is now "Mario Edwards Jr." and "Dante Fowler, Jr." is now "Dante Fowler Jr.".

## Data Import
    >>> import pandas as pd
    >>> df = pd.read_csv('combine.csv')
    >>> len(df)
    4947
    >>>
