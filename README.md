# scalerts
A Python program that serves as a news aggregator. It sources the articles from the hyperlinks of the RSS feeds given in a text file, stores the relevant information in an SQLite3 database and creates a .xlsx file with only the latest articles in it everytime it is run.

# Installation Instructions (For Windows)

#### Software required:
* `Python 3.0` and newer versions
* `SQLite3`
* Any Spreadsheet viewer that can open *.xlsx files.

#### Required Modules for Python:
You can easily use `pip install <module_name>` to install these modules.
* `feedparser` module
* `sqlite3` module
* `openpyxl` module

#### To run the program using `Command Prompt` do the following:
* Add python to your `PATH` variable.
* Migrate to folder containing the file `scalerts.py` by using `cd` command.
* Now you can use `python scalerts.py` to run the file.
 
# Information

* The `urlList.txt` file can be edited to add URLs. Since the program pulls the URLs from this file, it should under no circumstances be deleted.
* You can find instructions on how to make dedicated RSS feeds for any topic using Google alerts [here](https://support.google.com/alerts/?hl=en#4815700).
* On running the program for the first time, one will see the accompanying database file `scalerts.db` and excel file `scalerts.xlsx` being created.
 * The database file will be appended with new incoming content and keep increasing in size. _This file should not be deleted casually_.
 * The excel file will be overwritten with new posts everytime the program is compiled. *Maintaining daily backups of this file is the user's responsibility*. Do not save backups with the same name( and in the same folder) as the `scalerts.xlsx` file.
