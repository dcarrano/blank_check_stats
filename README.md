# Real Nerdy Stats

This Python project uses the [Rotten Tomatoes Scraper](https://github.com/pdrm83/rotten_tomatoes_scraper) package to compile information about movies discussed by the podcast [Blank Check with Griffin and David](https://audioboom.com/channel/Blank-Check).

Running the **blank_check.ipynb** Python notebook will create a dataframe called **blank_check_df** and a file called **blank_check.csv** with the compiled stats. (I've also uploaded these contents to [Google Sheets](https://docs.google.com/spreadsheets/d/10tcmKe5NDox3cyafL8EGctQ5L4p7ANUljjqVX1BW_TQ/edit?usp=sharing).)

To run the notebook, you'll need the Rotten Tomatoes Scraper package, and all the packages upon which it in turn is dependent. You'll also need the [Pandas](https://pandas.pydata.org/) package.

**Blank Check** covers both directors (on its main feed), and franchises (on its [Patreon feed](https://www.patreon.com/blankcheck/posts)). This can lead to duplication... for instance, James Cameron's film **Aliens** has been covered both as part of a Cameron series, and as part of an **Alien** franchise series. For certain uses -- e.g., calculating the average Rotten Tomatoes score of directors and/or franchises -- this is the desired behavior. There are other situations where you may wish to drop the duplicates.

Note that, because of the way that Rotten Tomatoes Scraper is set up, only movies covered by the "director" series will have info regarding year of release and box office. Also, Rotten Tomatoes' box office info is very spotty in general... e.g., **Star Wars** is listed as making $365, and sometimes even recent movies like **Aloha** have no info.

Smell ya later, fartheads!
