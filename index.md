
Ierg4230 project summary 

 

Ho Ho Ming 1155127665 

Project Name: Pet Sleep Monitor 

 

-Introduction: This is a IoT devices with a chip and camera build inside which will help us to monitor the sleeping of our pet. 

 

-Target user: Anyone have a pet and care about the health of their pet. The pet should be a creature that sleep in a certain place. I.e., hamster, dog, turtle, reptile, bird. (not for cat) 

 

-Objective: To let the user track the sleep period of their pets. With the big data analysis in the server, we may know if there are any health concerns of the pet by monitoring their sleep time and pattern. With the camera inside the devices, the owner may also monitor their pet by real time video streaming. Also, after knowing the pet’s sleeping habits, the owner will know when the best time is to play with their pets. Nevertheless, this IoT device may integrated with other devices such as auto food feeder, to feed the pet only when they are active so the food will not pollute the environment or a smart pug to turn off the light automatically when the pet is going to sleep. Final, we may not if the pet shit or not by analysis the real time image so we can clean the place as soon as possible. 

 

-Why this is an idea only project:  This device needs to actively track whether the pet is sleeping or not in a certain place. The sensor given will only detect the in and out motion not what the pet is doing. Also, they will not work at certain pet with low body temperature such as turtle or reptiles. The most versatile sensor to do the sleep recognize of different is a camera. 

 

-System architecture/building blocks 

This IoT project contain three buildings blocks. 

In the devices side, there will be a IoT devices combined with a camera and a chipset. The user needs to place it in the right place, connect it to a power source and turn it on. The user also needs to register an account in our website. 

 

In the cloud side, the device continues send whether the pet is sleeping and the time stamp to the cloud. The cloud will allow function for real time tracking, real time video streaming, big data analysis and machine learning prediction. 

 

In the user interface side, the user may know all the information and prediction via website in any platform. It can also be a mobile apps or a medical report to the clinic. 

 

-How it works: 

How the Arduino can know the pet is sleeping or not:  

The Arduino should preform edge detection to find all the edge point in the image captured by the camera every five seconds. It then generates an array that contain all the edge points in the image. When this array continues to change, it means the pet is moving. When it remains unchanged, it means the pet is not moving and is in sleep. 

 

How the cloud server predicts health.  

At the beginning, due to the lack of data, we can do simple pattern matching. If someone’s pet varies too differently from the average pattern obtain from others and itself in the past. There is high probability something goes wrong. The average pattern can be obtained by sampling data from another pets or made by scientist. 

After having enough data, we can unlock the power of machine learning and big data analysis to help us. 

 

 

 

-IoT elements 

big data analysis when there are massive users. With lot of users, we may improve the detection on the hidden health concerns by analysis the big data. 

cloud computing. The device only sends out the meta data and will not do any computing. All the computing stuff is done in the cloud. 

battery powered. The device can power by battery or solar plane. 

Communication gateway. The device uses WIFI to transfer the data. 

user interface. The resulting data may present in different such as graph in mobile apps or a formal medical report in the desktop website. 

machine learning. When there are enough data, we may use machine learning to improve the sleep recognize and the predict the relationship between sleeping period and health of the pet more preciously. 

 

-Features/functions 

sleep monitoring. 

Real time video streaming though phone. 

Health report every week. 

Auto alarm after the pet shitted. 

Integrate with other smart home devices such as auto food feeder and lights. 

 

-components used 

A camera 

ESP8266 (to do the sleep recognize locally, if chose to do it in the server, the transfer data will be large and use lot of energy) 

A Power sources (any kind will make it) 

A case (to protect your pet) 

Some wires to connect the components 

 

-Applications 

In home for any personal customers. 

In animal clinic or hospital for better medical cares and monitoring. 

In pet hotel, to let the owner know the status of their pet as a selling point. 

In the lab to help the experiment relative to animals going better. 

In the wild to help scientist to study the behavior of wild animals better. 

 

-Highlights, challenges, limitations 

Develop an algorithm to detect the sleeping of the pet that run locally in the Arduino will be hard due to the limited computing recourses. 

The camera module may use too much power, it is very important to lower the power used by the camera 

The study and analysis of the relationship between sleep and health need a large amount of investment. 
