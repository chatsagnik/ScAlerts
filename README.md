# scalerts
A Python program that aggregates articles from provided RSS feeds, stores the articles in an SQLite database and creates a .xlsx file with only the latest articles in it. 


--Technical Details--

1. scalerts.py takes one RSS feed URL and parses it. scalertsgoogle.py shows how it can be modified to take multiple RSS feeds and parse them accordingly.

2. The urllist[] in scalertsgoogle.py contains various RSS feeds which were created using alerts.google.com.

3. The program utilises the feedparser module to parse the RSS feeds, the sqlite3 module to establish a connection with a database that stores the articles and the openpyxl module to create a new .xlsx file which contains only the latest articles provided by the feed.

4. On running the program for the first time, one will see the accompanying database file and excel file being created. Henceforth, the database file will be appended with new incoming content and keep increasing in size while the excel file will be overwritten with the new posts.

5. If user wants to use the excel file for a later time they must make a backup as there is a high probability of the file getting overwritten. They may also access the database directly in such cases.

6. If for a particular day the feeds come up with lesser articles than the preceding day, then the excel file will not be completely overwritten, and may contain some news article from the previous day lower down in the file. The Datestamp column is in place to prevent confusion about the publication date of a particular post.

7. This was created to help content writers access relevant news in one place.
