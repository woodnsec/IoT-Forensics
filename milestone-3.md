# Progress Report April 25th, 2019
**Capstone:** IoT Forensics  
**University:** University of Nebraska at Omaha  
**Members:** Elisabeth Henderson, Ashley Leedom, Amber Makovicka, Ronald Ramirez, & Nathan Wood   

- [Overview](#overview)
- [Outcomes](#outcomes)
- [Hinderances](#hinderances) 
## Overview
(insert brief overview of efforts made)

## Outcomes
(brief overview of outcomes - what did you achieve?)

##### *just some ideas from two sources I found that we might be able to apply to our project*
Reading 1 - [Security Analysis of the Amazon Echo](https://courses.csail.mit.edu/6.857/2017/project/8.pdf)
* Summary - As the title states, authors of this reading conducted a security analysis on the Amazon Echo.  They defined an ideal security policy which included three main goals, confidentiality, integrity, and availability. This security policy is then used to reference the vulnerabilities they would later attempt. The authors conducted Sound, network, and API attacks. Here are a couple examples that the authors conducted that could be useful to us.   
 
   + Sound-based Attacks – When placing orders, Amazon prevents users from buying stuff by having a user enter a 4-digit PIN. The authors wrote a script to brute-force the 4-digit PIN since Amazon doesn’t limit the number of attempts when ordering
   
   + Network Attacks – The authors used Wireshark to conduct a man-in-the-middle attack, to intercept and record the traffic. They were able to retrieve the MAC address of the device and but weren’t able to decrypt the data portion of the packets.  


Reading 2 - [Digital forensic approaches for Amazon Alexa ecosystem](https://www.sciencedirect.com/science/article/pii/S1742287617301974)

* Summary - In this paper, the authors focused on the digital forensics based on the Intelligent Virtual Assistant (IVA) Alexa’s Ecosystem. One of the points that I thought was interesting was pertaining to the database of the Alexa Mobile App. Using an Android device, the application uses two SQLite files called “map_data_storage.db” and “DataStore.db” where the first database contains the token information about the user who is logged in. And the data is deleted when a user signs out. The other database includes to-do and shopping lists. Nevertheless, the results when examining the database files showed that there was little information stored on the device. 


#### Hands on research with Google Home Mini device  
We setup a private WiFi network to conduct our study on the Google Home Mini IoT device. This was accomplished with a WiFi Pineapple device [https://wifipineapple.com/pages/nano](https://wifipineapple.com/pages/nano) to broadcast the network and do a packet capture (pcap) on the IoT device. 

![WiFi Pineapple + GH Mini](/GHmini-pcap.PNG?raw=true "The WiFi Pineapple web interface and packet capture")

WiFi Pineapple = 172.16.42.1
Google Home Mini = 172.16.42.248

Unfortunately for our research the application traffic was encrypted and we were unable to find valuable data from the pcap. The application data was sent via the http-over-tls protocol meaning it was encrypted before it was transmitted. This is good for security but not so much for our research project. 

![GH Mini pcap application data](/GHmini-pcap-application-data.PNG?raw=true "The packet capture highlighting the encrypted application data")

Luckily we are able to access the [developer portal](https://developers.google.com/actions/smarthome/logging) of the Google Home Mini - this allows us to see what a law enforcement officer might be able to subpoena for logs in a criminal investigation. 

![GH Mini stackdriver logs](/GHmini-stackdriver-logs.PNG?raw=true "The stackdriver application logs from Google Cloud Platform")

An example of what the logs look like from the Google Cloud Platform is available in our repo here: [GHMini-stackdriver-logs.json](/GHMini-stackdriver-logs.json). Logs are cleaned by Google to only share the failure type/error reason with the developer, not a detailed trace. For forensic purposes this is sufficient. **(citation needed - Nate)** Additional details on how to collect logs as a developer are available at the [developer portal](https://developers.google.com/actions/smarthome/logging). 

Google directs US based agencies to their [Transparency Report Help Center](https://support.google.com/transparencyreport/answer/7381738?hl=en). This page details what requirements are set for the legal process for user data requests. The website CAL-MASS [Google LE Guide](https://calmass.org/?wpdmpro=google-le-guide) article indicates there are exigent circumstances which allow law enforcement agencies to expedite the legal process to request user data. 

#### Hands on research with Google Home Mini device Part 2 - Using IoT Inspector from Princeton
* Open-soure tool letting our group inspect IoT traffic through a browser. 

Using IoT Inspector, an open-source tool which lets us inspect IoT traffic developed by Princeton, we wanted to see what information would be collected using our Google Home Mini. When running IoT Inspector it captures all the devices on the network.

![myDevices_home](https://user-images.githubusercontent.com/45551925/56472764-5049e400-6428-11e9-810e-18eaa2037af0.png)

IoT Inspector makes it easy monitor the traffic of the Google Home Mini by having different views such as the following:

* Default view -  displays all the traffic monitored   
* Companies view - displays company names the device contacted   
* Ads/Trackers view - displays ad/tracking services the device contacted   
* No Encryption view - displays cases where device sent or received plain HTTP traffic   
* Insecure Encryption view - displays cases where device interacted with Internet using insecure or outdated encryption   
* Weak Encryption view - displays cases where device interacted with Internet using weak encryption   

Below are a few images of the data that was captured when using the Google Home Mini for about 30 minutes. During these 30 minutes, we asked the Google Home Mini a variety of questions such as “What is the weather like today?” and also the Mini to play music on YouTube. 

* #### Default View
<img width="718" alt="googleMini_iot_default" src="https://user-images.githubusercontent.com/45551925/56472785-9bfc8d80-6428-11e9-8741-a7591fc264d2.png">

* #### Companies View  
<img width="728" alt="companies_View_googlemini" src="https://user-images.githubusercontent.com/45551925/56473176-e7189f80-642c-11e9-8d01-7bdcdeb3f719.png">

* #### Ads/Trackers View   
<img width="1156" alt="adsview_googlemini" src="https://user-images.githubusercontent.com/45551925/56473202-45de1900-642d-11e9-96be-ca515932b2ad.png">

* https://iot-inspector.princeton.edu/

 #### Hands on research with Ubertooth 
 We set up an [Ubertooth One](https://github.com/greatscottgadgets/ubertooth/wiki/Ubertooth-One) environment using a Ubuntu VM designed for Bluetooth sniffing, an obsolete, available Android phone, and IoT devices. The IoT devices used were a Garmin HR+ and Metawear CPRO. (The Android phone available was mostly arbitrary, since we were just interested in capturing the Bluetooth packets to analyze.)  
 
 Within the tmp/ folder we created a folder named "Capture/" to hold Packet Capture (PCAP) files generated to later open and analyze in Wireshark. To do this, the following command was used in the terminal while in the tmp/ folder: "sudo ubertooth-btle -f -c ./Capture/[device].pcap". The "-f" flag is used to follow connections, and "-c" is used to tell the command where to save the file with what name.  
  
  The video below was recorded during a capture of Bluetooth packets between the Android phone and Garmin HR+. Packets are captured very quickly and information on the screen runs by too quickly for a human to read, however when making a Bluetooth connection, the packets run by faster. Following the established connection, the scrolling of packets returns to the pattern it was before.
  
 [![Video demonstration of Garmin HR+](https://i.imgur.com/UdgoMz8.png)](https://use.vg/5wPFS7)  
  
  At the end of the video, the file saved from the packet capture, 'garmin1.pcap' is opened in Wireshark. Using a string search, we can find the connection request packet, "CONNECT_REQ". This includes the MAC addresses of the devices used. It is worth noting the endian format of the MAC addresses are reversed when listed on Wireshark and on the phone/IoT devices. On a phone, it would list the Bluetooth MAC address as aa:bb:cc:dd:ee:ff, whereas on Wireshark it appears as ff:ee:dd:cc:bb:aa.  

![Wireshark screenshot](https://i.imgur.com/RXeJxax.png)  
(TODO: Analyze the packets captured.)

#### Hands-on Research with FTK Imager, Autopsy, and XRY
To do hands-on research with more traditional forensic tools such as FTK Imager, Autopsy, and XRY, a test bed using a Garmin wearable, Google Home Mini, Metawear, and a mobile device was set up. The Garmin is a wearable that records the user’s heart rate, steps taken, stairs taken, and when prompted GPS location as the user exercises outdoors. The device also has a mobile app that was downloaded on the phone. An account was set up with Garmin and the device was connected to the phone. A weekend was spent getting data on the device and phone. One teammate wore the device and periodically went out for “runs” to collect GPS data. The Google Home Mini and Metawear were also connected to this mobile phone and were periodically used over the weekend. The Google Home Mini was asked questions and instructed to create events. The Metawear was used to capture some data, however, when the teammate attempted to save the data, it errored out and was not uploaded to Google drive.  

The first test done with these devices was an attempt to connect them to FTK Imager to get an image of these devices, just as the first step would be in a traditional investigation involving a hard drive. The Google Home Mini was not recognized by FTK Imager and the Metawear does not have USB connection capabilities. However, surprisingly, the Garmin device was recognized by FTK Imager and a bit-for-bit image was created for that device. The image was then analyzed using Autopsy, a free forensic tool. Most of the files stored on this device have a “.FIT” file extension. This is Garmin’s proprietary file format. We were able to find an application called GPXSee that can read and display this file format, but only if there is GPS data in the file. With this application, we were able to see the exact routes taken by the teammate when they turned on the GPS function. In addition, we could see their speed and heart rate at all points along the route. Most interestingly, was the one deleted file found. At the end of a workout, the user has the option to save or discard the workout. Two of the workouts done were discarded. One was presumably overwritten by subsequent workouts (of which there were 2) the other, which was the last entry before data acquisition, was recovered and viewable using GPXSee. While we were not expecting it, we were able to gather a lot of data from this device.  

The second test done with these devices was pulling the data from the phone using XRY and using that as a proxy to get the data from the device. For this test, XRY Version 7.11 was used to create a full logical image of the mobile device. The image was then exported, and Autopsy was used to examine the files. The phone had been factory reset before the data propagation portion of this test, so there was not a lot of data on the phone itself. However, data was found from the Garmin device and Metawear. The only data found from the Google Home Mini was that there was a Google Home Mini connected to the mobile device and the events created using voice commands. No logs of the conversations or searches requested were found. According to Google, these logs would be found on their servers through the user’s Google account (CITE). The records created using the Metawear that were not saved properly were recovered from the phone. The records for the Garmin were the most informative. These included the user’s profile information (gender, weight, height, etc.), daily summary information (total steps, max, min, and average heartrate, etc.), and activity information (activity type, start date, start location, duration, etc.). Unfortunately, this data did not include the exact route taken by the user. While that data is shown on the app, it seems it is uploaded to the user’s account and only available online. This, and with the Google Home Mini, is where investigators might have to use cloud forensics to get all the data they might need for a case.    


## Hinderances
* Google Home Mini network traffic was encrypted using the http-over-tls protocol. This indicates little to no forensic data is available from the device itself nor the network it resides on.  
* Bluetooth works by working on three different channels between 2402-2480MHz, usually referred to as channel 37, 38, and 39. When capturing Bluetooth packets with the Ubertooth One between the Android phone and IoT devices, it had to be on the correct channel to capture. At times it would not be on the right channel to capture packets and the device would need to be reseated.  
* We had to try many phones before we found one that could interface with XRY. This tool has a specific list of phone models and operating systems it can work with. We had to try a few different phones before we could get any data off the device using XRY. With the limited number of phones we had at our disposal, we were not able to find one that we could do a full bit-for-bit extraction on, but we did have one that could be used for a full logical.  
* The data stored on the Garmin is in a proprietary file format. The files can be converted to CSVs, but they are not easily read in that format.  
* Many of these devices interact with the cloud so some of the data cannot be acquired using just traditional digital forensics or mobile forensics. Unfortunately, cloud forensics is outside the scope of this project so that data was not collected.  
 
