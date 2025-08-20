---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

#layout: home
layout: default
---
Argyle Square is a small park located in the center of Melbourne, Australia only walking distance from Melbourne Museum. With it’s about 17.250 m<sup>2</sup> it is home to some local Italian atmosphere according to [Tripadvisor](https://www.tripadvisor.com/Attraction_Review-g255100-d11883026-Reviews-Argyle_Square-Melbourne_Victoria.html).
To dive more into when people stay at this culture park the [blix-visits](https://data.melbourne.vic.gov.au/explore/dataset/blix-visits/information/?sort=datetime) dataset and [benches usage data](https://data.melbourne.vic.gov.au/explore/dataset/guppy/information/?disjunctive.dev_id) dataset from [the city of Melbourne opendata](https://data.melbourne.vic.gov.au/) have been used. The blix data counts the number of phones. The bench data monitors when people use two benches at the park and the temperature.

<div style="display: flex; justify-content: center; margin-bottom: 20px;">
  <div class="image-container">
    <iframe src="My final project codes\city park map.html" width="600px" height="550px" style="border:none; margin-bottom: 20px;" title="Argyle Square city park map"></iframe>
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    <small>Figure 1: <strong>Argyle Square city park map.</strong> <em>Explore the map by hovering over the marks and clicking on them.</em></small>
  </p>
</div>
 
## Do people stay at the park or use it for passing through to work?
Firstly, we will have a look at what time most people visit the park. For this the blix (mobile phone counter) data is used meaning the data is from 2022 till mid-2024.

<div style="justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="My final project codes\visits_sum_total_polar.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    <small>Figure 2: <em>LOVE IT!!!</em></small>
  </p>
</div>

Here it is shown that at 1 o’clock pm is where the park is the busiest with people with mobile phones. At 5 o’clock in the evening is also fairly busy and overall, the busiest time of day in this small park is from 8 am till 8 pm. It is very clear to notice that there are not a lot of people at the park at night and especially from 3 am till 5 am. This seems very reasonable when considering people are normally sleeping at night not at parks. 

The data above only counts the number of phones (wifi-devices) and not the time spend at the park. So, this could also tell us a bit about when rush-hour is since people might just be passing through the park to go to work and back. However, according to [soho](https://soho.com.au/articles/peak-traffic-hours-melbourne), [3aw](https://www.3aw.com.au/melbournes-peak-hour-now-lasts-for-six-hours-a-day/) and locals rush hour in Melbourne is around 6:30 am till 9 am and from around 3:30 pm till 6 pm.
Let’s investigate when the park is most crowded and therefore at what time people tend to stay at the park for longest and isn’t just passing through the park to go somewhere else.

<div style="justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="My final project codes\visits_sum_dwell_polar.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    <small>Figure 3: <em>LOVE IT even more!!!</em></small>
  </p>
</div>

When comparing the two plots with each other it is clear to notice that people are actually spending time at the park when visiting. However, the rush hours do show up a bit when comparing the plots. At around 9 am and 5-6 pm there are more people at the park, and most likely just passing through the park, than staying at the park. 

To look more into if rush-hour has anything to do with when people are at the park the follow bar chart, where the total amount of visitors at the park is sorted into weekdays, is produced.

<div style="justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="My final project codes\visits_weekdays_bar_chart.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    <small>Figure 4: <em>LOVE IT even more and more and more!!!</em></small>
  </p>
</div>

Overall, there is not a big difference in the day of the week but over the course of the 2 and a half years this dataset spans, there is a difference of about 35,000 people between Monday and Friday. If people were just using the park for walking through to get to work one would expect to see more visits on weekdays. This is not the case which is a final factor for confirming that people actually do use/stay at the park.

## Why are people staying at that time of day?
Another interesting factor about when people are staying at that park is to look at the average dwell time per person (or actually per device). 

**Insert plot here** Figure 5

It is very interesting to notice that the highest average time a person stays at the park is at 4 am, and it is for 7 hours. When looking at the Argyle Square city park map the range of the mobile phone counter is 30 meters therefore the reasoning for the 7 hours at night can’t be explained by the department buildings around the park. [Tripadvisor](https://www.tripadvisor.com/Attraction_Review-g255100-d11883026-Reviews-Argyle_Square-Melbourne_Victoria.html) states there once were a mafia gang called the Carlton Crew and they had their base at the Carlton district which is where Argyle Square park is located. When looking more into the history of mafia, according to [State Library Victoria]( https://ergo.slv.vic.gov.au/explore-history/rebels-outlaws/city-criminals/gangland-war) the history of the Carlton Crew was most active 1998 to 2006 where The Gangland War took place. Even though crime in the area has decreased since then the Carlton district is still a place where crime takes place as reported by [Red Suburds](https://redsuburbs.com.au/suburbs/carlton-vic/#overview). This could explain why some individuals tend to stay at the park for a long period of time doing nighttime.

## The use of the benches at the park
Each bench has two sensors monitoring when the bench is at use. The interactive plot below shows at what time of day people are sitting at the bench for the longest. 

<div style="justify-content: center;">
  <p style="margin-left:5px; margin-top: 10px; font-style: italic;">
    <small>Figure 6: <em>Argyle Square city park map. Explore the map by hovering over the marks and clicking on them.</em></small>
  </p>
  <div class="image-container">
    <iframe 
      src="My final project codes\Bokeh_plot_benches.html"
      width="900" 
      height="380"  
      style="border:none;" 
      title="Argyle Square city park map">
    </iframe>
  </div>
</div>

One can tell there are no obvious favorites of which of the two benches to use. Both benches have an odd outburst. For bench 1 located closest to the Piazza Italia sensor 2 has an outburst at 12 o’clock and for the other bench it is sensor 3 which has an outburst at 5 o’clock pm. We do see from the polar plot (figure number) a larger dwell time at the park at 12 o’clock and more visitors at 5 pm which could explain the two outbursts. However, it could also be errors in the data.

The use of benches is highest in the afternoon and evening. When further investigating the plot (figure number (the one above)) there is a slight favor in bench 2 from 3 pm till 8 pm. This might be due to the location of the benches. The following plots display the temperature at the bench/sensor.

<div style="justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="My final project codes\bench_sensor1_histogram.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    <small>Figure 7: <em>LOVE IT even more and more and more!!!</em></small>
  </p>
</div>
<div style="justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="My final project codes\bench_sensor4_histogram.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    <small>Figure 8: <em>LOVE IT even more and more and more!!!</em></small>
  </p>
</div>

One can differently tell that bench 2 has higher temperatures than bench 1. It is interesting to notice that for bench 1 people tend to use the bench more when the temperature is around 15-19 degrees but for bench 2 it is around 17,5-20,5 degrees. Furthermore, when only looking at the temperature it seems people like to sit more at bench 1 where the temperature is lower.

How many of the people who visit the park are using the benches. See plot below.

<div style="justify-content: center;">
  <p style="margin-left:5px; margin-top: 10px; font-style: italic;">
    <small>Figure 9: <em>This is an interactive plot. Try and hover over the datapoint to see the dates of the observation. The year can be chosen in the drop-down menu in the top left corner. Furthermore, use the zoom icon to zoom in at the data point you find interesting. By clicking the spinning circled arrows, the plot will resent to its original state. The blue dots are the blix/mobile phone counter data, and the crosses are the bench data.</em></small>
  </p>
  <div class="image-container">
    <iframe 
      src="My final project codes\Bokeh plot with combined data for 2022 and 2023.html"
      width="900" 
      height="500"  
      style="border:none;" 
      title="Argyle Square city park map">
    </iframe>
  </div>
</div>

Firstly, it is clear to notice that most of the people who are visiting the parks aren’t using the two benches. One also very quickly notice for 2022 the two outliers Sunday the 2nd of October and Saturday the 15th of October. On the 2nd of October 2022 [Festival Indonesia]( https://www.eventfinda.com.au/2022/festival-indonesia/melbourne/carlton) has held at the park. The festival seamed to had been a success because according to figure … the following year on the 8th of October [the festival was held again]( https://busycitykids.com.au/melbourne-calendar-events/2023/10/8/festival-indonesia-at-argyle-square) and this time around 3000 more people attended according to figure … .
On the 15th of October 2022, the other outlier in the plot, the [Fringe parade]( https://melbournefringe.com.au/wp-content/uploads/2022/07/Parade-Info-Pack-for-Participants-.pdf) has walking Lygon street which as shown on the Argyle Square city park map is located right along one of the sides of the park. Furthermore, when hovering over some of the other smaller outliers for 2022 where more people than usual visit the park one will notice that most of these dates are between the 10th and the 24th of December.  This is most likely due to the [pop-up roller skating rink](https://participate.melbourne.vic.gov.au/neighbourhoods/carlton/christmas-roller-rink) that was set up doing that time. 
Please note there are two visible outliers in 2023 as well which I unfortunately haven’t been able to find a clear explanation for. 

# In Summary
Argyle square seems to be a popular place with almost 1 million people visiting a year. They are not just walking through the park to get to work but they also tend to stay favorably from mid-day till evening and on Fridays. There are at least two benches at the park which are mostly used from 11am till 22 pm and when the temperature is at around 15-21°C. There are big events throughout the year taking place in the park which attract many people. Lastly, a few people tend to stay the longest at the park doing the nights. 