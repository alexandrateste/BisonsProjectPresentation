---
title       : On The Bisons Tracks!
subtitle    : Following the Dunn Ranch Prairie bisons' daily wanderings
author      : Alexandra Teste
job         : October 2015
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
url         :
        assets: ../assets/img
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- &twocol w1:50% w2:50%

## Dunn Ranch Prairie Bisons


<blockquote>&ldquo;Let's take a trip to the wild and follow bisons for a while ...&rdquo;</blockquote>

<br>

*** {name: left}

Over the past few years, bisons have been re-introduced to the [Dunn Ranch Prairie](http://www.nature.org/ourinitiatives/regions/northamerica/unitedstates/missouri/dunn-ranch-prairie-flyer.pdf), in Missouri. Some of them were collared by [Stephen Blake](http://www.peoplebehindthescience.com/dr-stephen-blake/)'s team, and data on their movements were collected and graciously made available to the public through the [Movebank](https://www.movebank.org/panel_embedded_movebank_webapp).


The ["On the Bisons Tracks!"](https://teal13.shinyapps.io/BisonsProject) application is a tool that allows the user to explore this dataset through a map visualization and the display of travel characteristics directly extracted from the dataset and computed from it.


*For the sake of speed and ease of understanding, the data available for exploration through this app correspond to those collected in 2013. The animal IDs have been rescaled to integers between and 1 and 12.*

*** {name: right}

![app](TrackingData.png)

--- &twocol w1:50% w2:50%

## Features

*** {name: left}

["On the Bisons Tracks!"](https://teal13.shinyapps.io/BisonsProject) allows the user to:

* Track animals, on a map, throughout the selected day
* Run cumulative distance travelled calculations and display
* Obtain information on the animals' ground speed over time.

This app is interactive with a date picker and 2 checkboxes. It updates automatically when a new date is selected.

*Note: The user should wait for a few seconds when first opening the app, to allow for the map to appear. Once it is visible, the user can interact with the app and navigate to the Documentation tab.*

*** {name: right}


```
## [1] "May 15, 2013"
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 

*Plot produced at the time of "slidification".*

--- 

## Documentation

Full documentation is additionally available in a separate tab. It provides explanations on:

* The source of, and context in which, the data used in the application were collected
* The transformations they underwent
* The calculations that run behind the scenes.

![app](Documentation.png)

--- .class #id 
<style>
em {
  font-style: italic
}
</style>

## Acknowledgements & Beyond

<br>

I would like to thank Stephen Blake and his team for making these data publicly available, and the Movebank for creating such a great source of animal tracking data!

<br>

This application can be used with any other tracking (i.e. location-based) dataset, and adapted to display the metrics relevant to the scientific project in question.

<br>

As any project completed in a short amount of time, this application could benefit from improvements. I would more particularly like to add an inter-bison distance computation, to exploit the gender data available in the dataset, and to provide weekly/monthly/yearly statistics on the distances travelled and most favorite gathering grounds.


