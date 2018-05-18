# classifyWines
Code for the FS2018 course Machine Learning

## Sources
Basic statistic with plotly: https://plot.ly/python/basic-statistics/

## Useful commands
`source activate conda35` to use conda environment in mac terminal

Data management
merging with panda: merged = pandas.merge(left, right, on='key')

Show basic data
# redwine_overview_table = figureFact.create_table(redwinedata[0:5])
# py.iplot(redwine_overview_table, filename='winequality-red')


#convert median to panda series
red_median = pandas.Series(list(red_median))
white_median = pandas.Series(list(white_median))

#convert from type: series to new type dataframe to be able to plot. 
basicStats = pandas.DataFrame({'feature':red_mean.index, 'mean_red':red_mean.values, 'mean_white':white_mean.values, 'std_dev_red': red_stdev.values, 'std_dev_white': white_stdev.values, 'median_red': red_median.values, 'median_white': white_median.values })