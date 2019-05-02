##security Monitor Readme.


##Some basic information 


###The concept that I have decided to base my project on is Homeowner security. I wanted to prove a proof on concept that anyone can take their smartphone and turn it into a fully capable iot device that will monitor their house whilst their at work or asleep.



I wanted to prove that any device that met the basic specifications could in theory be used as a homeowner security device. 
I decided to use a smartphone in this instance as it has all the available sensors required to carry out the functions that would be needed to acheive the end goal.

The device mounts to a door where it waits for a stimulus, the device in theory could range from anything including an Arduino board, raspberry pi, apple iPhone or android smartphone. The device for proof of concept will mount to a door where it waits. Once a vibration is present the user should be able to visualise the data, save the data and be alerted of such an occurrence. 

###What works?
As of now the device is able to record vibrations using the phones onboard accelerometer. It can also send these readings to a cloud based server where these readings can be viewed and later saved. 
I have also been able to modify an application that connects the users phone to an external program known as Evothings where the raw sensor data can be seen as well as the users location. However sending a notification to the user letting them know of a disturbance has been hit and miss.


As of now I have found 2 methods in acheiving the goals that I have set out above. One is to use IBMS cloud system to contextualise, visualise and extract data from a smartphone. The other is to use EvoThings in conjunction with an application in the format of html document that is provided in this GitHub repo.

For both of these methods all that you will require is a modern smartphone, internet connectivity and a computer.





#Setting up IMB cloud.

(1) #What is the IMB Watson platform.
The IBM Watson IoT Platform is a fully managed, cloud-hosted service that makes it simple to derive value from Internet of Things (IoT) devices. When combined with the IBM Bluemix platform, Watson IoT provides simple, but powerful application access to IoT devices and data. You can rapidly compose analytics applications, visualization dashboards, and mobile IoT apps. Create IoT applications that feed insights to your backend enterprise applications.


(2)Firstly you will need to do the following.

(3)Open your favorite browser and go to Bluemix. If you are an existing Bluemix user, log in as usual. Once you signed up to Bluemix, click this link to create the Watson IoT Platform service in Bluemix.
Type a name for your service and click Create button as shown below,
Observe that now you can add and manage iot devices.

(4) Now create a device type, each device that is connected will be associated with a device type. An example of a device type could be andoird device, pc etc.

(5) Continue with the setup inputing your prefered fields, REMEMBER to write down these fields or screenshot them as you will need them later for mqtt connecivity later on.

(6) Next you will have to generate a code that is unique to the service that you are creating REMEMBER to save this code. 

(7) Now you can download any mqtt application onto your phone, input the details that you have screenshotted earlier on into the empty fields. The device as well as the IBM system should now be in sync with one another.

(7) You shoud see a flow of data from the phone to the computer.

(8) In this recipe we demonstrated how to setup an IBM Watson IoT Platform Organization, create a Device Type and register a Device using theIBM Watson IoT Platform dashboard. Also, you can use the IBM Watson IoT Platform ReST API, or the Client Libraries to create the Device Type and register Devices in IBM Watson IoT Platform.

#Setting up EvoThings Application

#What is EvoThings?
Evothings Studio is a set of development tools, designed for development of mobile apps using web technologies. Evothings Studio is specifically designed for development of apps for the Internet of Things. The application has been adapted from a EvoThings Developer who has made an application for a similar purpose. https://github.com/hammadtq/Evothings-Demo-Apps



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
