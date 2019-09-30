# Data Visualization Final Project Proposal - Nuclear Explosions

This is a final proposal for my data visualization project using the Nuclear Explosions dataset.

## Data

The data I propose to visualize for my project is the [Nuclear Explosions dataset](https://github.com/rfordatascience/tidytuesday/tree/master/data/2019/2019-08-20). This dataset contains information about nuclear explosions that were deployed from 1945 to 1998. The data contains information such as:
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

## Prototypes

I have made many starting prototypes that show different aspects of the data. 

[![image](https://user-images.githubusercontent.com/23533132/65432224-d22fa600-dde8-11e9-9b88-8ccab1eb3b3d.png)](https://beta.vizhub.com/rachelhahn/ecc92c07391341999d4017de7f9eb3b5)

This visualization is a simple bar chart that shows how many deployments there were per country. My issue with this visualization is that it does not show time, location, or any specific information about each deployment. 

[![image](https://user-images.githubusercontent.com/23533132/65432562-6e59ad00-dde9-11e9-9b53-aa212f3ca3fa.png)](https://beta.vizhub.com/rachelhahn/64c679fe2e3e4b248e97da26d7b6e011)

This map is a start of the kind of visualization that I want to create for this dataset. It shows the latitude and longitude of where each deployment was. The region is also shown when the user hovers over each deployment. I would like there to be an accurate world map behind these locations as well as more information shown about each deployment; maybe size of the circle will be based on the magnitude of the explosion. Lastly, I would like there to be something to show time; maybe a time bar that the user can slide to change the year. 

[![image](https://user-images.githubusercontent.com/23533132/65433064-5171a980-ddea-11e9-9b17-4c68015e19d7.png)](https://beta.vizhub.com/rachelhahn/6564525e2c61457d96b282b152241ffe)

This visualization is a line chart that shows how many nuclear devices each country has deployed compared to the other countries throughout time. I enjoy this visualization because it shows what has happened over time; we can see how the number of deployments changed over time. I think this visualization is also missing the aspect of where each deployment went off (latitude and longitude). 

[![image](https://user-images.githubusercontent.com/23533132/65433552-410dfe80-ddeb-11e9-8870-f43ec268bdbe.png)](https://beta.vizhub.com/rachelhahn/951ee3e6df1446929164d6833eefc92d)

This visualization is a better version of my first prototype; it is a stacked bar chart that shows how many devices each country deployed with the added information of what the purpose of each deployment was. However, it is still missing the location and the time that I want to show in my final visualization. 

[![image](https://user-images.githubusercontent.com/23533132/65882660-72467b80-e363-11e9-8389-bd3bea6603c9.png)](https://beta.vizhub.com/rachelhahn/cdee1169ba054ac09d5483965a49e338)

This visualization is an improvement of my second prototype; it shows a world map with little circles that represent the latitude and longitude of each deployment. The map is the Mercator projection. The biggest problem with this prototype is that the points are off by a small fraction (down and to the left) however it fits much better on the Mercator projection over the Natural Earth projection. When the user hovers over each point, they can see the specific latitude and logitude of that deployment. This is a base protoype that I would like to build upon for my final project. 

## Questions and Tasks

I want my final visualization to answer the following questions:

 * What countries deploy the most nuclear devices and how does it compare to the other countries? (Show this with the color of the dots)
 * Where are the devices deployed compared to which country deployed them? (Show this with a map of each deployment and color of the dot)
 * How does the deployment area for each country change over time? (Show this with a time slider)
 * What is the magnitude of each deployment compared to the other deployments? (Show this with size of dots)
 * What is the purpose and type of each device deployed? (Show this with more information in a box when the user clicks on the dot)

## Sketches

![image](https://user-images.githubusercontent.com/23533132/65434458-d78eef80-ddec-11e9-8061-52e28af5426b.png)

This image shows my three original sketches for the nuclear dataset. 

1. This first sketch shows a simple bar chart that would show which countries deployed the most nuclear devices compared to the other countries. This sketch definitely answers the first question but none of the other ones because it doesn't show time or location. 

2. The second sketch is a scatter plot that shows how many deployments each country had over time. This sketch answers the first question and adds the time aspect to it. However, it still does not show location. 

3. The third sketch is a map that shows where each deployment happened and has the user interaction of being able to change the year as well as click on a circle to see more information. This sketch answers the questions 1, 2, 3, and 5. It still does not answer the 4th question. This sketch is very close to what I would like my final visualization to be. 

## Ideas for Interactions

I have many ideas of what interactions I might want to have in my final project. Some of these ideas are inspired by the video [Effective Visualization](https://canvas.wpi.edu/courses/18991/pages/video-effective-visualization?module_item_id=330143). 

Note: I am planning the base visualization to be a map of the world with circles for each nuclear deployment. 

 * To change time, I would like to have an interaction with a timeline (specifically a line chart) below the map that shows the number of nuclear deployments per year compared to the map bounds. The user would be able to slide a vertical line through the chart to change the circles (deployments) on the map to show what happened in that year. The user would also be able to zoom in and out on the map and the chart would change based on the bounds of the map.
 * I would like to have an interaction that would allow the user to filter what the map shows. Specifcally, I would like the user to be able to filter the map based on type of deployment or purpose of deployment. Example: the user could filter to show deployments that were only due to combat.
 * I would like to have an animation of each explosion that will animate whenever the user changes the year (see the first point). In the animation, I would like the circle to be highlighted (to stand out) and start big based on the size of magnitude and then shrink to a normal circle size. All the circles would end with the same size; magnitude would only be reflected at the beginning of the animation. Imagine the animation as being similar to what an explosion might look like from a birds-eye view.  
 * The last interaction idea is to bring up a menu of information whever the user clicks on a circle. The menu would contain all the extra information a user might want to learn about that specific deployment such as, the source of who reported it as well as the depth of the explosion. 

## Open Questions

There are a few things that I am doubtful that I can complete:

 * I am not sure how to show a world map behind my latitude and longitudes with the correct positions based on the map projection. 
 * I am not sure how to create a line chart that the user could interact with to change the year to see the change of data
 * I am not sure how to create an "information box" that would pop up when the user clicks on a circle
 * I am not sure how to create a filter menu
 
 Other than these things, I think I could create something that would answer all my questions!
 
 ## Schedule of Deliverables
 
 1. Finish the base map with circles for each deployment. **Delivery Date: October 2nd**
    - Align the circles with latitude and longtiude perfectly.
    - Color the circles based on which country deployed that device.
    - If the animation does not work: Change the size of each circle based on the magnitude of each deployment. 
 2. Create the time interaction. **Delivery Date: October 9th**
    - Create the line chart that shows number of deployments per year that has a vertical line that the user can slide to change what year the map is showing. 
    - (REACH GOAL) Allow the user to zoom in and out on the map and have the line chart change based on those bounds. 
 3. Create the information box that will pop up when the user clicks on a deployment. **Delivery Date: October 16th**
 4. Create a filter menu to allow the user to filter based on purpose of deployment and type of deployment. **Delivery Date: October 23rd**
 5. (REACH GOAL) Create the explosion animation that will animate when the user changes the time. **Delivery Date: October 30th (Final Project Due)**






