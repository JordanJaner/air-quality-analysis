# air_quality_analysis
The files contained within this repository utilize the EPA AQS API to analyze PM2.5 concentrations and AQI in California, New York, and Texas. These states were chosen due to their size and wide distribution in the United States. 

The investigative team was interested in the following three questinos:
Are there differences between California, New York, and Texas in PM2.5 concentrations?
Are there significant differences in PM2.5 concentrations for California between different latitudes? 
Are there any seasonal trends or trends throughout the year in PM2.5?


From the original 2020 PM 2.5 annual dataset provided by the EPA, records for CA, NY and TX pollutant standard
“PM2.5 annual 2012” and event type “Events Excluded” and “No Events” were selected, in order to derive a set of
comparble arithmetic mean values of pollutant levels at each sensor.

Google Maps API was used to create a heatmap of annual average PM2.5 levels in California, Texas and New York in 2020.
A visual scan of the heatmaps suggests that the average daily PM2.5 concentration in California was worse than in
Texas and New York. In fact, the annual arithmetic mean in California was 11.96, in New York, 8.81, and Texas, 6.35.
The most updated EPA PM2.5 upper limit standard is an annual mean of 12 micrograms per meter cubed. In 2020, as a state, California
was very close to this upper limit.

After removing dates associated with an event and removing outliers from the data, California showed higher range of air PM2.5 conentartion as depicted by the box plots compared to New York and Texas. Even though california had higher range of PM conecnatrion and greater daily maximum concentrations, it showed similar median concentration as compared to Texas. New York on the other hand had significantly lower median PM2.5 concentration.
Air Quality Index showed to be mainly driven by PM2.5 concentration as presented in the scatterplots above, with california's AQI reaching to 80.

After creating the dataframe that was specific to just California locations, analysis shows that there is really no correlation between the arithmetic means and latitudes in California. This highlights that the latitude does not affect the level of PM 2.5 in California. The second visual shows the correlation between the first max values recorded and the fourth/final max values recorded for the specific site. Based on the visual there is a strong positive correlation which can tell us that depending on the size of first max value it can be projected that the fourth max value will have a similar size.

Based on the visual of the box plots and the statistics associated with each quarter, it seems likely that there is an effect of time of year on PM2.5 concentrations in California, New York, and Texas. Comparing Q2 to Q3, the mean Microgram/Cubic meter concentrations of PM2.5 in Q3(14.72) is more than double the concentrations in Q2(7.1). This is not simply due to outliers. The upper quartile of Q2(8.91) is less than the lower quartile of Q3(10.02). Due to the magnitude of difference between these measurements, there is strong evidence that time of year may be a significant factor in PM2.5 concentration. As these states represent three distinct geographic locations in the United States, further research may indicate that this phenomenom is present across the United States.
