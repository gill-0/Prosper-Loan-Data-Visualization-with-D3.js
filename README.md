# Prosper-Loan-Data-Visualization-with-D3.js
Interactive Javascript Visualization on Loan Data


## Summary 

Prosper is a peer-to-peer lending company marketed as an alternative to banks that launched in 2006. I explored a Prosper loan data set of over 100,000 observations and 81 variables to create a meaningful visualization with D3.js and dimple.js. My visualization examines the relationship of how Prosper Credit Ratings and Prosper Scores changed with interest rates over the years. 

## Final Visualization

Below is a block link that will render my visualzation.

http://bl.ocks.org/gill-0/raw/e1d7421efec070b38084edad64c7955f/

## Design

### Data Points

I grouped the data points by year, prosper credit rating, and prosper score. This allowed enough data points to see a clear trend while not cluttering the visualization.

I though a scatter plot would best represent the data since both the x and y axis are continuous. 

### Animation

By exploring how the data changed over the years I found an interesting trend, so I decided to incorporate an animation that stepped through the years in order to clearly see how the data changed. 


### Color

I used a diverging 7 point color scheme in order to clearly show the difference in Prosper credit ratings.

### Years Bar Chart

Through the years Prosper has continued to grow. I thought that adding bar charts representing the number of loans would give more context to the visualization. By changing the bars color, they also double as an indicator for the selected year.  

### Changes made from Feedback

I changed the scales from decimal points to percentages as I think that it is more intuitive for readers who were confused.

I changed the scales from decimal points to percentages as I think that it is more intuitive for readers who were confused.  I also changed the x and y axis labels to be more clear. 

  Y axis: Estimated Return -> Investor's Estimated Return 
  X axis: Annual Percentage Rate -> Borrower's Interest Rate (APR)

I expanded the introduction to give readers a clearer understanding of the trend in the visualization.

I had mixed feedback on the year's bar chart, but I think it is relatively simple/clear. I can also make it clearer through the introduction.

## Feedback

### Feedback Person 1

Doesn’t quite understand what the x and y axis show.

Likes the year bar on the side.

Thinks the colors make the visualization clear.

### Feedback Person 2

Knows very little about interest rate and APR.

Takeaway is that high risk seems to be associated with high reward (except with the HR credit rating) and predictions were better over time.

Thinks the bars on the right showing sample size are confusing. Is there a significant difference between 2k and 30k? Grammar error in introductory paragraph.

### Feedback Person 3

I don’t actually ever say APR is Annual Percentage Rate.

Confused when I said “Prosper Ratings and Scores” in the introductory paragraph. They weren’t sure if Prosper Credit Rating was the same as Prosper Rating so I should clear that up.

I should elaborate on my title of the visualization by explaining the visualization more with a few sentences.

## Files

HTML file containing final data visualization

```{r}
prosper_data_visualization.html
```

HTML file containing initial data visualization

```{r}
prosper_data_visualization_initial.html
```

R markdown document containing exploraty data analysis

```{r}
prosper_loan_explore.Rmd
```
Loan Summary Data File

```{r}
prosper_summary.tsv
```

## Resources

https://www.orchardplatform.com/blog/alphabetic-ratings-and-numeric-scores-on-prosper/

https://www.prosper.com/about-us/wp-content/uploads/Performance_Update_January2017.pdf

http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control

https://github.com/d3/d3-scale-chromatic

http://colorbrewer2.org/#type=diverging&scheme=BrBG&n=7

https://discussions.udacity.com/t/custom-tooltip-legend-order/189042/6

https://techcrunch.com/2008/11/26/sec-outlines-its-reasoning-for-shutting-down-p2p-lender-prosper/
