
Ierg4230 project summary 
 

Ho Ho Ming 1155127665 

Project Name: Pet Sleep Monitor 


-theoretical backup

How can we detect the object in the image is moving?:

By using the result of "Jain, R. and H. Nagel, “On the Accumulative Difference Pictures for the Analysis of Real World Scene Sequences,” IEEE Tran. on Pattern Anal. Mach. Intell., pp. 206-221, 1979.". We can use the frame differencing method, which make use of  image subtraction operator to subtract the image sequence and compare them for moving object detection. 

Or we may use temporal differencing from "Weiming Hu, Tieniu Tan, Liang Wang, and Steve Maybank, “A Survey on Visual Surveillance of Object Motion and Behaviors,” IEEE Trans. on Systems, Man, and Cybernetics—Part C: Applications and Reviews,vol. 34, no. 3, pp. 334-352, August 2004". Which detect the moved object by apply pixel wise difference calcuation within some frames

Doing simple optic flow calculation will also work. By "Burton, Andrew; Radford, John (1978). Thinking in Perspective: Critical Essays in the Study of Thought Processes. Routledge. ISBN 978-0-416-85840-2.". We can know that optic flow method can let us know the pattern of relative motion in a scence. In "Aires, Kelson R. T.; Santana, Andre M.; Medeiros, Adelardo A. D. (2008). Optical Flow Using Color Information (PDF). ACM New York, NY, USA. ISBN 978-1-59593-753-7.". We know that it can be used to detect moving object.

In this project, due to the low resolution of the camera, the poccessing power used for calcuation will be very small. Also, we dont need to do the object detection all the time, instead, we may do it every 5 second.

How the machine learning work?:

At the beginning, due to the lack of data, we can do simple pattern matching. If someone’s pet varies too differently from the average pattern obtain from others and itself in the past. There is high probability something goes wrong. The average pattern can be obtained by sampling data from another pets or made by scientist. 

After having enough data, we can unlock the power of machine learning and big data analysis to help us. The "Nilsson N. Learning Machines, McGraw Hill, 1965." and "Duda, R., Hart P. Pattern Recognition and Scene Analysis, Wiley Interscience, 1973" already proof that machine learning is powerful in pattern classification.



-Why this is an idea only project:  
Only a camera can do the job I want, there are no alternative.
This device needs to actively track whether the pet is sleeping or not in a certain place. The sensor given will only detect the in and out motion not what the pet is doing. Also, they will not work at certain pet with low body temperature such as turtle or reptiles. The most versatile sensor to do the sleep recognize of different is a camera. 
 
 
 
-Introduction: This is a IoT devices with a chip and camera build inside which will help us to monitor the sleeping of our pet. 
 
 
 
-Target user: Anyone have a pet and care about the health of their pet. The pet should be a creature that sleep in a certain place. I.e., hamster, dog, turtle, reptile, bird. (not for cat) 

 

-Objective: To let the user track the sleep period of their pets. With the big data analysis in the server, we may know if there are any health concerns of the pet by monitoring their sleep time and pattern. With the camera inside the devices, the owner may also monitor their pet by real time video streaming. Also, after knowing the pet’s sleeping habits, the owner will know when the best time is to play with their pets. Nevertheless, this IoT device may integrated with other devices such as auto food feeder, to feed the pet only when they are active so the food will not pollute the environment or a smart pug to turn off the light automatically when the pet is going to sleep. Final, we may not if the pet shit or not by analysis the real time image so we can clean the place as soon as possible. 

 

-System architecture/building blocks 

This IoT project contain three buildings blocks. 

In the devices side, there will be a IoT devices combined with a camera and a chipset. The user needs to place it in the right place, connect it to a power source and turn it on. The user also needs to register an account in our website. 

 

In the cloud side, the device continues send whether the pet is sleeping and the time stamp to the cloud. The cloud will allow function for real time tracking, real time video streaming, big data analysis and machine learning prediction. 

 

In the user interface side, the user may know all the information and prediction via website in any platform. It can also be a mobile apps or a medical report to the clinic. 

 
 

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
