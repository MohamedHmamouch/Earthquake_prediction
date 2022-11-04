# Earthquake_prediction

<p> This project consists in predicting earthquakes based on Tweets.The center has extracted the data using the tweeter api. The automatic earthquake detection algorithm was calibrated before the other analyses (geo-inference and analyses (geo-inference and classifications), and is therefore based on a more restricted data set. 
For this purpose, They used data collected by BRGM on Twitter during the period from March 28, 2015 to March 25, 20161 with the addition of data collected on April 7 and 8 April 2014 following the Ubaye earthquake (representing a total of 53205 tweets).In parallel, we characterized the French seismicity that occurred over the same period, completed on a case-by-case basis by the worldwide earthquakes that gave rise to French-speaking on Twitter </p>

<h3> 2- BRGM they used an algorithm for detection :</h3> 

<p> First processed the data by aggregating a "timeline" with a time step of 
(i.e. counting the number of tweets exchanged each minute), and computed, every minute 
calculated the STA (Short Term Average) parameters (i.e. the instantaneous value of the 
minute, i.e. the instantaneous value of the timeline) and LTA (Long Term Average = average of 
Tweets / minute over a sliding window of one hour).
Based on the study of seismicity catalogs, we then looked for earthquakes that have 
given rise to testimonial posts on Twitter, and assigned to each of them a value of the 
STA/LTA couple corresponding to the time of the first activity peak (see Table 1 and Table 2).
Moreover, each of the messages posted in the minutes after the occurrence of these earthquakes and 
obviously written by witnesses (having felt the tremors or not) have been "tagged" manually (nearly 
"manually tagged (nearly 2500 tweets) to distinguish between first-hand and 
first hand and the others - a priori less significant -.
We decided to implement the Twitter earthquake detection technique proposed in 
the 2011 paper by Earle et al2 which is inspired by traditional seismic detection methods, and is based on the 
seismological detection methods, and is based on exceeding an ATS threshold value that is linearly dependent 
of LTA :</p>

