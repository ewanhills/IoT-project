##security Monitor Readme.


###Some basic information 


The concept that I have decided to base my project on is Homeowner security.

I wanted to prove that any device that met the basic specifications could in theory be used as a homeowner security device. 
I decided to use a smartphone in this instance as it has all the available sensors required to carry out the functions that would be needed to acheive the end goal.

The device mounts to a door where it waits for a stimulus, the device in theory could range from anything including an Arduino board, raspberry pi, apple iPhone or android smartphone. The device for proof of concept will mount to a door where it waits. Once a vibration is present the user should be able to visualise the data, save the data and be alerted of such an occurrence. 

###What works?
As of now the device is able to record vibrations using the phones onboard accelerometer. It can also send these readings to a cloud based server where these readings can be viewed and later saved. 
I have also been able to modify an application that connects the users phone to an external program known as Evothings where the raw sensor data can be seen as well as the users location. However sending a notification to the user letting them know of a disturbance has been hit and miss.


#As of now I have found 2 methods in acheiving the goals I have set out above one is to use IBMS cloud system to contextualise, visualise and extract data from a smartphone. The other is to use EvoThings in conjunction with an application in the format of hmlt that is provided in this GitHub repo.
























#Setting up EvoThings Application

#What is EvoThings?
Evothings Studio is a set of development tools, designed for development of mobile apps using web technologies. Evothings Studio is specifically designed for development of apps for the Internet of Things.


(1) Firstly install evo things onto your computer.
https://evothings.com/

(2) Next download the evoThings application onto you android or apple device.

(3) After both have installed, go to evo things on your computer, agree to the terms and conditions and proceed to the next step.

(4) In order to connect your phone and computer together you will need to generate a key like so that you will enter into the smartphone,
the devices will then attempt to connect to one another.


![](C:\Users\Ewan Hills\Pictures-keycode.png)


(5) The devices should have connected successfully.

(6) Next drag and drop the html file from this repo into your EvoThings program.

(7) REMEMBER it is important that if you wish to receive sms notifications you must change the number in the html file to 
a number of your preference.

(8) The html allpication will now appear on your computer where you can now run the application from.

(9) The application will detect mocement and should alert you of movement via sms on your mobile phone.
