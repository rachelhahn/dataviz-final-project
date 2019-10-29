# Data Visualization Final Project - Nuclear Explosions

This is the final project for my data visualization course using the Nuclear Explosions dataset. I go through the dataset and the type of information it has, my original sketches, my initial prototype visualizations, my favorite visualizations (which ends in what I consider to be my final visualziation), the questions that the final visualization answers, my timeline of completed tasks, and finally what future work I would like to complete for this visualization. 

## Data

The data I visualized for this project is the [Nuclear Explosions dataset](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-08-20). This dataset contains information about nuclear explosions that were deployed from 1945 to 1998. The data contains information such as:
 * the date and year of the explosion, 
 * a unique ID, 
 * which country deployed the device, 
 * where the device was deployed, 
 * the source who reported the deployment, 
 * the latitude and longitude of where the device was deployed, 
 * magnitude and depth of the deployment, 
 * the purpose of the deployment, 
 * the name of the device, and
 * the method of deployment.
 
 
## Sketches

Before I started to create prototype visualizations, I sketched out some ideas for the nuclear dataset I had chosen. 

![image](https://user-images.githubusercontent.com/23533132/65434458-d78eef80-ddec-11e9-8061-52e28af5426b.png)

1. This first sketch shows a simple bar chart that would show which countries deployed the most nuclear devices compared to the other countries. This sketch definitely answers the first question but none of the other ones because it doesn't show time or location. 

2. The second sketch is a scatter plot that shows how many deployments each country had over time. This sketch answers the first question and adds the time aspect to it. However, it still does not show location. 

3. The third sketch is a map that shows where each deployment happened and has the user interaction of being able to change the year as well as click on a circle to see more information. This sketch answers the questions 1, 2, 3, and 5. It still does not answer the 4th question. This sketch is very close to what I would like my final visualization to be. 

## Prototype Visializations

Over the course of this class, I made many prototype visualizations that show different aspects of the data. I built my final visualization off of these prototypes. 

[![image](https://user-images.githubusercontent.com/23533132/65432224-d22fa600-dde8-11e9-9b88-8ccab1eb3b3d.png)](https://beta.vizhub.com/rachelhahn/ecc92c07391341999d4017de7f9eb3b5)

This visualization is a simple bar chart that shows how many deployments there were per country. My issue with this visualization is that it does not show time, location, or any specific information about each deployment. 

[![image](https://user-images.githubusercontent.com/23533132/65432562-6e59ad00-dde9-11e9-9b53-aa212f3ca3fa.png)](https://beta.vizhub.com/rachelhahn/64c679fe2e3e4b248e97da26d7b6e011)

This map is a start of the kind of visualization that I wanted to create for this dataset. It shows the latitude and longitude of where each deployment was. The region is also shown when the user hovers over each deployment. I would like there to be an accurate world map behind these locations as well as more information shown about each deployment; maybe size of the circle will be based on the magnitude of the explosion. Lastly, I would like there to be something to show time; maybe a time bar that the user can slide to change the year. 

[![image](https://user-images.githubusercontent.com/23533132/65433064-5171a980-ddea-11e9-9b17-4c68015e19d7.png)](https://beta.vizhub.com/rachelhahn/6564525e2c61457d96b282b152241ffe)

This visualization is a line chart that shows how many nuclear devices each country has deployed compared to the other countries throughout time. I enjoy this visualization because it shows what has happened over time; we can see how the number of deployments changed over time. I think this visualization is also missing the aspect of where each deployment went off (latitude and longitude). 

[![image](https://user-images.githubusercontent.com/23533132/65433552-410dfe80-ddeb-11e9-8870-f43ec268bdbe.png)](https://beta.vizhub.com/rachelhahn/951ee3e6df1446929164d6833eefc92d)

This visualization is a better version of my first prototype; it is a stacked bar chart that shows how many devices each country deployed with the added information of what the purpose of each deployment was. However, it is still missing the location and the time that I want to show in my final visualization. 

[![image](https://user-images.githubusercontent.com/23533132/65882660-72467b80-e363-11e9-8389-bd3bea6603c9.png)](https://beta.vizhub.com/rachelhahn/cdee1169ba054ac09d5483965a49e338)

This visualization is an improvement of my second prototype; it shows a world map with little circles that represent the latitude and longitude of each deployment. The map is the Mercator projection. The biggest problem with this prototype is that the points are off by a small fraction (down and to the left) however it fits much better on the Mercator projection over the Natural Earth projection. When the user hovers over each point, they can see the specific latitude and logitude of that deployment. This is the base protoype that I used to build upon for my final project. 

## Favorite Visualizations 

To create my final project, I made 3 visualizations that built off of each other, each time making my visualization better. 

[![image](https://user-images.githubusercontent.com/23533132/67777497-340eab80-fa38-11e9-8720-5437b098581e.png)](https://beta.vizhub.com/rachelhahn/bfed5cbc1e4446af858141647fffd8b4)

This first visualization built off of the last prototype shown above. The world map behind the points (deployments) uses a Natural Earth projection. When the user hovers over each point, they can see the name, latitude, and logitude of that deployment. The size of each point directly corresponds to the magnitude of the explosion (the bigger the explosion, the bigger the point)! The color of each point also corresponds to which contry was responsible for the deployment of that nuclear device. The user can interact with the color legend; when one element of the legend is hovered over, the map will only show those points. Lastly, the user can click a specific deployment and see more information about that deployment in the bottom left corner.

[![image](https://user-images.githubusercontent.com/23533132/67777643-65877700-fa38-11e9-9613-277e0cd46308.png)](https://beta.vizhub.com/rachelhahn/0faa59883f5f4ca580f6a005694dccc1)

This visualization was built off the first visualization. It has the same interactions with the points and the color legend, but now also allows the user to filter what points they want to see. There are two filter menus at the top of the map which allows the user to filter the shown deployments based on purpose of deployment and type of deployment. For example, this specific image shows the deployments that were part of a weapons deployment program and that were deployed through an airdrop.

[![image](https://user-images.githubusercontent.com/23533132/67777876-c57e1d80-fa38-11e9-9d3f-c6b5441175f2.png)](https://beta.vizhub.com/rachelhahn/dac8f591b5fb43558d595d344feec54a)

This last visualization is what I consider to be my final project. It has the interactions mentioned above with the points, color legend, and the filter menus as well as a histogram at the bottom of the map to show how many nuclear events there were each year. The user can interact with the histogram to use a "brushing" technique; they can select a timeframe within the histogram and move it left or right to see the different deployments over time. For example, this specific image only shows the deployments between the years 1960 and 1965 based on the selected timeframe within the histogram. 

## Questions and Tasks

My final visualization answers the following questions:

 * What countries deploy the most nuclear devices and how does it compare to the other countries? (Shown with the color of each point)
 * Where are the devices deployed compared to which country deployed them? (Shown with a map of each deployment location as well as the color of each point)
 * How does the deployment area for each country change over time? (Shown with the histogram and brushing technique)
 * What is the magnitude of each deployment compared to the other deployments? (Shown with size of each point)
 * What is the purpose and type of each device deployed? (Shown when the user clicks on a point to see more information as well as the dropdown filter menus)
 
 ## Schedule of Deliverables - All Completed! 
 
 1. Finished the base map with circles for each deployment. **Delivery Date: October 2nd**
    - Aligned the circles with latitude and longtiude perfectly.
    - Colored the circles based on which country deployed that device.
    - Changed the size of each circle based on the magnitude of each deployment. 
 2. Created the information box that pops up when the user clicks on a deployment. **Delivery Date: October 9th**
 3. Created filter menus that allow the user to filter what is shown on the map based on purpose of deployment and type of deployment. **Delivery Date: October 16th**
 4. Created a histogram under the map that shows number of deployments per year. **Delivery Date: October 23rd**
 5. Created the time interaction (brushing) with the histogram. **Delivery Date: October 30th (Final Project Due)**
    - The histogram under the map allows the user to select a specific time frame where the map will only show deployments from that timeframe. The user can slide that selection through time to see how the map changes over time. 

## Future Work

1. Have an animation of each explosion based off of the magnitude. The animation would start when the user uses the brushing technique with the histogram. 
2. Allow the user to zoom in and out on the map and have the histogram change based on those bounds. 
3. Have the histogram change when the user changes what is selected through the filter menus.




