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
    Figure 1: <strong>Argyle Square city park map.</strong> <em>Explore the map by hovering over the marks and clicking on them.</em>
  </p>
</div>

<div style="justify-content: center;">
  <p style="margin-left:5px; margin-top: 10px; font-style: italic;">
    Figure 1: Argyle Square city park map. Explore the map by hovering over the marks and clicking on them.
  </p>
  <div class="image-container">
    <iframe 
      src="My final project codes\city park map.html"
      width="800" 
      height="500"  
      style="border:none;" 
      title="Argyle Square city park map">
    </iframe>
  </div>
</div>
 
## Do people stay at the park or use it for passing through to work?
Firstly, we will have a look at what time most people visit the park. For this the blix (mobile phone counter) data is used meaning the data is from 2022 till mid-2024.

<div style="justify-content: center;">
  <div style="display: flex; justify-content: center; align-items: center;">
    <img src="My final project codes\visits_sum_total_polar.png" style="width: 120%">
  </div>
  <p style="margin-left:5px; margin-top: 10px;">
    Figure 2: <em>LOVE IT!!!</em>
  </p>
</div>

Here it is shown that at 1 o’clock pm is where the park is the busiest with people with mobile phones. At 5 o’clock in the evening is also fairly busy and overall, the busiest time of day in this small park is from 8 am till 8 pm. It is very clear to notice that there are not a lot of people at the park at night and especially from 3 am till 5 am. This seems very reasonable when considering people are normally sleeping at night not at parks. 

The data above only counts the number of phones (wifi-devices) and not the time spend at the park. So, this could also tell us a bit about when rush-hour is since people might just be passing through the park to go to work and back. However, according to [soho](https://soho.com.au/articles/peak-traffic-hours-melbourne), [3aw](https://www.3aw.com.au/melbournes-peak-hour-now-lasts-for-six-hours-a-day/) and locals rush hour in Melbourne is around 6:30 am till 9 am and from around 3:30 pm till 6 pm.
Let’s investigate when the park is most crowded and therefore at what time people tend to stay at the park for longest and isn’t just passing through the park to go somewhere else.

