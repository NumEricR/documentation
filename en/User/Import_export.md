---
language: English
currentMenu: import
subTitle: Import and export data
---

# Import and export data
## Import

To import data in wallabag, go to the page **Configuration**.

### Caution

Data import can be a **demanding process** for your server. Hence, it is done in two steps:

* Insertion of the URL in the wallabag database
* in the second step, the retrieval, for each article, of its full content.

These two steps cannot be done concurrently, because it let us the possibility to import thousands of links, but today, wallabag does not have sufficient technical capabilities to do this task automatically.


### From Pocket
#### Export your data from Pocket

From your Pocket account, go to the options.
TODO

#### Import your Pocket data

From the configuration page of wallabag, section **Import**, select the file `ril_export.html` generated by Pocket, then click on **Import**.
Wallabag only insert these links in the database. Now, you have to get the content of each article.

For this, click on `Click to finish import`: wallabag will fetch the content of 10 articles at a time.

TODO

TODO new ticket: why when a click is done, this does not load in a loop? I believe this was doing this ping @mariroz

### From Instapaper
#### Export your data from Instapaper

TODO

#### Import your Instapaper data

TODO

### From Readability
#### Export your data from Readability

TODO

#### Import your Readability data

TODO

### From wallabag

Since you can export your data from wallabag (see below), it is of course possible to re-import them.

In the import form, select your wallabag-exported file (format JSON). Start the import, et voilà.

Unlike the above imports, this process is shorter because all the data (title and content of the articles) are already included in the file. Hence wallabag does not have to access each URL. However, the import file is necessarily bigger.


### From a HTML or JSON file

TODO

## Export
It is possible to export your data from the page **Configuration** of wallabag. Several reasons to do this:

* re-install of wallabag
* leave the Framabag service to install your own wallabag
* a user with an account on a multi-user wallabag want to have his/her own wallabag installation
* ...

This will lead you to download a file [at the JSON format](http://fr.wikipedia.org/wiki/JavaScript_Object_Notation).  
As detailed above, you can import this file in wallabag.
