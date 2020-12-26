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

Then do the programming part in Node-RED and also make connections to MongoDB.


