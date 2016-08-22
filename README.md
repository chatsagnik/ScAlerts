# scalerts
A feed aggregator built in Python.
It sources the articles from the hyperlinks of the RSS feeds given in a text file, stores the relevant information in an SQLite3 database and creates a .xlsx file with only the latest articles in it everytime it is run.

# Installation Instructions (For Windows and Ubuntu)

#### Software required:
* `Python 3.0` and newer versions
* `SQLite3`
* Any Spreadsheet viewer that can open *.xlsx files.

#### Required Modules for Python:
You can easily use `pip install <module_name>` on Windows or `sudo pip install <module_name>` on Ubuntu to install these modules.
* `feedparser` module
* `openpyxl` module

#### To run the program using `Command Prompt` do the following:
* Add python to your `PATH` variable.
* Migrate to folder containing the file `scalerts.py` by using `cd` command.
* Now you can use `python scalerts.py` to run the file.

#### To run the program from `Terminal` do the following:
* Migrate to folder containing the file `scalerts.py` by using `cd` command.
* Use the `python scalerts.py` to run the file.
 
# Information

* The `urlList.txt` file in the repository contains a list of RSS feed URLs. *This can and should be edited to add your own URLs*. Since the program pulls the URLs from this file, *it should under no circumstances be deleted*.
* The `scalerts.db` and `scalerts.xlsx` file in this repository are example database and spreadsheet files that were created using the `scalerts.py` program. *They should be deleted before the program is compiled for the first time*.
* You can find instructions on how to make dedicated RSS feeds for any topic using Google alerts [here](https://support.google.com/alerts/?hl=en#4815700).
* On running the program for the first time, one will see the accompanying database file `scalerts.db` and excel file `scalerts.xlsx` being created.
 * The database file will be appended with new incoming content and keep increasing in size. _This file should not be deleted casually_.
 * The excel file will be overwritten with new posts everytime the program is compiled. *Maintaining daily backups of this file is the user's responsibility*. Do not save backups with the same name( and in the same folder) as the `scalerts.xlsx` file.

## *Used by [AlCircle.com](http://www.alcircle.com/)
