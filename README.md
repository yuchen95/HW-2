Homework 2
================

THIS IS STILL A WORK IN PROGRESS
--------------------------------

You are currently in the GitHub repository (repo) for `HW-2`. You must have completed all the steps in [Setting Up](https://rudeboybert.github.io/MATH216/jekyll/update/2016/09/12/getting-started.html).

Learning Goals
--------------

-   

Homework
--------

1.  Follow the same workflow as in <a target="_blank" class="page-link"
    href="https://github.com/2016-09-Middlebury-Data-Science/HW-0#homework">HW-0</a> for HW-2.
2.  Do not submit a `HW-2.Rmd` file that does not knit.
3.  I anticipate you spending between 8-12 total (across all submissions) on this homework.

Data
----

Result of a Python script that scraped the OkCupid website. We consider 59K users who were:

-   members on 2012/06/26
-   within 25 miles of SF
-   online in the last year
-   have at least one photo

Their public profiles were pulled on 2012/06/30. i.e. only data that’s visible to the public. Also included are essay question response data in variables `essay0` through `essay9`. The codebook for the data is available [here](https://github.com/rudeboybert/JSE_OkCupid/blob/master/okcupid_codebook.txt). Note:

-   Usernames were excluded from data set. This is **not** a guarantee of de-anonymization.
-   Permission to use this data was granted from OkCupid.

Run the following code once to download the OkCupid data from GitHub into your `HW-2` RStudio project i.e. into your `HW-2` folder. After you run this, there should be a file `profiles.csv` in the same directory as all your `HW-2` files.

``` r
url <- "https://github.com/rudeboybert/JSE_OkCupid/blob/master/profiles.csv.zip?raw=true"
temp_zip_file <- tempfile()
download.file(url, temp_zip_file)
unzip(temp_zip_file, "profiles.csv")
```

Tips
----

1.
