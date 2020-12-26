# A Hong Kong smart city case based on AWS and Node-RED
An application that fetch data streams from https://data.gov.hk/, data analysis and correlation, as well as dashboards to present insights in relation to the selected smart city use cases.

This is also the programming assginment from HKU MSC CS COMP7503.

# requirements:  

Amazon AWS EC2 : 
A platform where we can set up our own instance and make connections to it.         

Node-RED: 
A programming tool where we can fetch data streams and do programming work. It also has the dashboard to present insights in relation to our smart city cases.           

MongoDB: 
A database that we use to store and analyze required data.            


# implementation:

1. connect to the AWS EC2 instance(by using ssh connection)            

eg. ssh -L 1880:localhost:1880 -L 27017:localhost:27017 -i XXXX.pem.txt ec2-user@XX.XX.XX.XX

2. connect to the Node-RED and programme

eg. url:   http://localhost:1880/

Then do the programming part in Node-RED and also make connections to MongoDB(the /.json file).


# our project work
We focus on the real-time weather information of Hong Kong.  The dashboards of our project are shown in the picture below.
![](https://github.com/Taossi/A-Hong-Kong-smart-city-case-based-on-AWS-and-Node-RED/blob/main/1.png)
![](https://github.com/Taossi/A-Hong-Kong-smart-city-case-based-on-AWS-and-Node-RED/blob/main/2.png)

There are mainly 4 different functions: basic weather information, radiation & air quality, rainfall and weather map.

In Basic Weather Information, it shows the current temperature, humidity and uvindex in Hong Kong Observatory and its update time. Also, based on the current weather situation, we use an automatic tip system to give some useful suggestions for people on going outside.

In Radiation & Air Quality, we firstly show the basic current radiation situation in Hong Kong. Then there is a chart showing air quality health index in every location in Hong Kong in the past 24 hours. In Rainfall part, we present the rainfall situation in 18 different places in Hong Kong during a period by a rainfall chart.

Finally, in Weather Map, we show a real-time Hong Kong map with many different dots. Each dot means a place. Blue dots present current rainfall situation in this place, while green dots store the temperature information in this place. We can check each dot to see the weather detail of this place.
