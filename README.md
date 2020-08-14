# WoSo Stats
This GitHub repository is for the WoSo Stats project, dedicated to collecting, analyzing, and distributing data about women's soccer from around the world. In this repository you'll find a variety of code, files, and documents relevant to our work.

Most of you are probably here because you want the advanced stats. To get right to it, run the following in R, which will create a `tbl_all` data frame in your working directory with a large collection of stats for each player in each game in the database. **You can also directly download the table [here](https://raw.githubusercontent.com/alfredomartinezjr/wosostats/master/data/summary/tbl_all.csv)**, for now, as this is not the intended final destination for this. Ideally it'll be hosted somewhere on the WoSo Stats site or on a cloud storage service like AWS S3.
``` r
source("https://raw.githubusercontent.com/alfredomartinezjr/wosostats/master/calc_stats.R")
```

You can more easily view the stats in [the WoSo Stats Shiny app](https://amj2012.shinyapps.io/wosostats/). It is a Shiny app, an interactive web app that runs on R.

The [resources](https://github.com/amj2012/woso-stats/tree/master/resources) directory is where to find necessary and helpful resources for how to log stats on your own and definitions for what is being measured and analyzed. While matches are not currently being actively logged, this is still useful if you want to go through and see how matches are logged and definitions for the stats in the tbl_all table.

The [data](https://github.com/amj2012/woso-stats/tree/master/data) directory is where to find the WoSo Stats database, for now. The raw Excel match logs can be found in [a public Google Drive folder](https://drive.google.com/drive/folders/13-8Ws14GougTk_FZBv4k-VUCaRyml1hj?usp=sharing). The data/database/ directory is a database of tables based on the Excel files, which are a result of running the lineups_to_db.R and excel_to_db.R scripts. This is not meant to be a permanent location for that database, hence the name, and the plan is to also move it off of Github and somewhere onto the WoSo Stats site.

Currently, our biggest database is for 2016 USWNT matches and for the 2016 NWSL season. While this project is still being occasionally worked on, matches are not being logged as regularly as in the past and it is more likely that this project will try to log and archive data from historical matches (pre-2016) as advanced stats have recently been tracked more regularly for certain women's soccer competitions.

The main Twitter account for this project where you'll find the most up-to-date info on recent news, stats, and overall developments is [@WoSoStats](https://twitter.com/wosostats). The website is at www.wosostats.com. Any questions about the project or how to join can be directed to the Twitter account or to Alfredo at wosostats.team@gmail.com.
