# scalerts
A Python program that aggregates articles from provided RSS feeds, stores the articles in an SQLite database and creates a .xlsx file with only the latest articles in it. 

The urllist[] in scalertsgoogle.py contains various RSS feeds which were created using alerts.google.com.

The program utilises the feedparser module to parse the RSS feeds, the sqlite3 module to establish a connection with a database that stores the articles and the openpyxl module to create a new .xlsx file which contains only the latest articles provided by the feed.

This was created to help content writers access relevant news in one place.
