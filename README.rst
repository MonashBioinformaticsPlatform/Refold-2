Rewrite of the REFOLD protein refolding database
=========================================================

**REFOLD is now retired** to a tropical island, to live out its days in a molten globule state surrounded by delicious chaotropes. 

**We've dumped the important data as TSV** format into **data/**, excluding Django-specific stuff and user data.
This should be enough to resurrect the project in some form if anyone felt so inclined, or the pull data into R or Python dataframes with the appropriate table joins and do stats / machine learning. There's no license here, but it would be safe to regard the data as Public Domain.

*Original README follows*

----

Formerly at http://refold.med.monash.edu.au

Security concerns on the former php4-based site have spurred this rewrite.

**Notes:**


* Currently only a read-only view of some database information. No ability for users to add/edit data.
* Requires an SQL database to be pre-loaded (i.e. django syncdb doesn't work for a blank database). This is due to the old database being used to create the Django models.
* Dependencies: django, django-completion (https://github.com/coleifer/django-completion/zipball/0.2.1), and south
* Buildout config for auto-dependency loading is coming, plus a guide to loading the autocomplete indexes
