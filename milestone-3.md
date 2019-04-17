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


Hands on research with Google Home Mini device
We setup a private WiFi network to conduct our study on the Google Home Mini IoT device. This was accomplished with a WiFi Pineapple device [https://wifipineapple.com/pages/nano](https://wifipineapple.com/pages/nano) to broadcast the network and do a packet capture (pcap) on the IoT device. 

![alt text](/GHmini-pcap.PNG?raw=true "The WiFi Pineapple web interface and packet capture")

WiFi Pineapple = 172.16.42.1
Google Home Mini = 172.16.42.248

Unfortunately for our research the application traffic was encrypted and we were unable to find valuable data from the pcap. Luckily we are able to access the [developer portal](https://developers.google.com/actions/smarthome/logging) of the Google Home Mini - this allows us to see what a law enforcement officer might be able to subpoena for logs in a criminal investigation. 

## Hinderances
(insert brief discussion of challenges encountered)
