
An analysis of hard drive data from the Backblaze which includes 15 Gig of data going back to 2013 including 90 columns of raw and normalized SMART hard drive statistics which may provide some leveraging to predicting hard drive failure. In particular the analysis would:
* apply survival analysis to these hard drives in order to predict failure rates with uncertainty estimates
* apply machine learning analysis (random forest, tensorflow/skflow) in order to predict pending hard drive failures
* apply correlation studies to Backblaze data combined with other data sources (user reviews, historical price data, serial number, hd manufacture date, manufacture location, crystal disk info, Acronis  drive monitor, WMI  etc.)
* generate a web tool that will tell users the probability their hard drive will fail
This project has potential, but in reality hard drives today are extremely reliable and most failures are stochastic. However, this may indicate that deeper more subtle statistical analysis with proper confidence interval handling is necessary. An advantage of the Backblaze data is that they use consumer grade hard drives (this is merely because they are cheaper) so combing their data with online retailers or other data sources could generate a novel hard drive metric. This is an interesting problem because hard drives are critical to computing and failures can be catastrophic and expensive. Data centers mitigate this risk through redundancy, but that is expensive and most consumes don’t have this ability. Summarily, low probability but high impact events like hard drive failure are interesting statistical events. 

[In addition there is a Heroku application with an interactive plot.](https://arcane-fortress-84192.herokuapp.com)
