# Progress Report (insert date here)
## Overview
(insert brief overview of efforts made)

## Outcomes
(brief overview of outcomes - what did you achieve?)

also list them out like this:
* outcome 1
* Difficult stuff for frameworks
  :(

## Hinderances
(insert brief discussion of challenges encountered)

## Ongoing Risks
(address your project risks identified from Milestone 1 and update them based on your current progress, this should be a table)


## Quick Notes: 

1. **Security of IoT Sensor Networks**  
**Authors:** Jeffrey Cichonski, Jeffrey Marron, Nelson Hastings  
**Date Published:** February 2019 (draft)  
**Published In:** [NIST website](https://www.nccoe.nist.gov/projects/building-blocks/iot-sensor-security)  
**Summary:** The Internet of Things (IoT) universe is continuously evolving and expanding as new products and technologies are introduced to the marketplace. IoT sensor networks—networks of small devices, or nodes that detect, analyze, and transmit physical data—are a prime example of this ongoing evolution. The National Cybersecurity Center of Excellence (NCCoE) at the National Institute of Standards and Technology (NIST) are partnering to develop a project to protect building management systems' IoT sensor networks.  
**Notes:**  This paper is not quite as on topic as previously thought for IoT forensics. It does have plenty of references to the topic and possible frameworks, however the paper is geared more towards a architecture overview for sensor networks and scenarios which theoritically test those networks. I think it will be good to reference while establishing what things should be checked in a IoT forensics framework.  

1. **Internet of Things Security and Forensics: Challenges and Opportunities**  
**Authors:** Mauro Conti , Ali Dehghantanha , Katrin Franke , Steve Watson    
**Date Published:** 2017    
**Published In/Citation:** Conti, Mauro & Dehghantanha, Ali & Franke, Katrin & Watson, Steve. (2017). Internet of Things Security and Forensics: Challenges and Opportunities. Future Generation Computer Systems. 78. 10.1016/j.future.2017.07.060.   
**Summary:** The authors of this literature begin to discuss the security and forensics challenges in the world of IoT. A few of the challenges the authors expand on are aspects such as authentication, privacy, and evidence identification, collection, and preservation. The authors then go on to conclude their literature with solutions they referenced from other publish papers.    
**Notes:**  Some things to talk about, because of the widespread of IoT devices which college and transfer data, security plays a big challenge. Security challenges mentioned in the reading : Authentication and Privacy.  

1. **A Generic Digital Forensic Investigation Framework for Internet of Things (IoT)**  
**Authors:** Victor R. Kebande and Indrakshi Ray  
**Date Published:** September 26, 2016  
**Published In:** 2016 IEEE 4th International Conference on Future Internet of Things (IoT) and Cloud (FiCloud)  
**Summary:** Kebande and Ray have developed a generic IoT forensic investigation framework that reliably supports digital investigations in IoT-based infrastructures. The framework complies with the ISO/IEC 27043:2015 international standard and provides a promising baseline for IoT forensic investigations.  
**Notes:** This paper compares existing models of digital forensics and IoT forensics - It has 3 categories of IoT forensics: Cloud, Network, and Device forensics. The Cloud forensics focuses on data generated in the cloud environment. Network forensics focuses on the communications of IoT devices. Device level forensics focuses on the digital evidence contained on the IoT devices, like memory, audio or video. 3 frameworks are compared against the proposed framework: Oriwo, Zawoad & Husan, and Perumal. 

1. **Digital Evidence Challenges in the Internet of Things**  
**Authors:** Robert Hegarty, David J. Lamb, Andrew Attwood  
**Date Published:** 2014  
**Published In:** Published in INC 2014  
**Summary:** In this paper, the authors begin to explain the rise of IoT devices. Examples such as intelligent home control systems to advanced city management systems, which produce and consume personal data. With the consumption and use of personal data, challenges arise. Thus, in order to help mitigate IoT challenges, the authors identify key areas that solutions should target.  
**Notes:** ...  

1. **IoT Forensic: Bridging the Challenges in Digital Forensic and the Internet of Things**  
**Authors:** Nurul Huda Nik Zulkipli, Ahmed Alenezi and Gary B. Wills   
**Date Published:** January 2017    
**Published In:** Conference: 2nd International Conference on Internet of Things, Big Data and Security 2017  
**Summary:** In this paper, the authors mention how these smart devices are used in many domains such as homes, transportation, and healthcare. However, these devices could be easily attacked because of the low-security mechanisms implemented and as a result could compromise legitimate data in an investigation. In order to help combat this issue, the authors propose two different approaches for the pre-investigation and implementation phases in forensics.  
**Notes:** This paper has great information on IoT forensics challenges that helps outline the difficulties in IoT. Some of the challenges mentioned are the following: The Investigation Framework, Diversity of Devices, and Lack of Standardization. The authors also talk about the sources of threats in IoT devices, which could help us during our Milestone 3 part of this project.   

1.  **Internet of Things Forensics: Challenges and Approaches**  
**Authors:** Edewede Oriwoh, David Jazani, Gregory Epiphaniou, and Paul Sant  
**Date Published:** 2013  
**Published In:** 9th IEEE International Conference on Collaborative Computing: Networking, Applications and Worksharing  
**Summary:** This paper mentions the various issues, threats, and attacks relating to IoT devices. It presents a realistic scenario of a malicious individual taking advantage of digital devices, including IoT devices. Important and relevant questions are asked as to how to respond and investigate the crime committed. Afterward it states the issues between traditional and IoT digital forensics, and follows with a recommended approach to handling the IoT devices.  
**Notes:** This paper is great for referencing a realistic scenario that involves many devices and really shows how complicated the investigation can get. It halso has a few useful tables with information about traditional and IoT digital forensics.

1. **IoT Forensics: Challenges For the IoA Era**  
**Authors:** Aine MacDermott, Thar Baker, and Qi Shi  
**Published In:** 2018 9th IFIP International Conference on New Technologies, Mobility and Security (NTMS)  
**Summary:** The authors coined a definition for IoT in the paper focusing on the interconnected infrastructur and utilities of existing devices among the existing Internet infrastructure. Issues are broadly defined for IoT forensics as being volume, variety, and velocity. The paper focuses on challenges of investigating crime scenes that involve IoT devices, such as the size of the object, location, relevance, legal/jurisdiction issues, blurry network boundaries/edgeless networks, and avaialble tools. Issues are presented in this paper with different categories of IoT based devices.  
**Notes:** The paper gives a good look at IoT forensics from an investigator point of view and presents numerous examples and issues with IoT forensics. 

1. **Internet of Things: The Need, Process Models, and Open Issues**  
**Authors:** Maxim Chernyshev, Sherali Zeadally, Zubair Baig, and Andrew Woodward  
**Published In:** IT Professional (Volume: 20, Issue: 3, May.Jun. 2018)  
**Summary:** This paper speaks about the complexity of extracting information from IoT devices. It can be uncertain where data is originating, where and how it is stored, and data attributes. The IoT infrastructure also can make it difficult to abide by standards in having a chain of custody since data can be very volatile and complex transit routes of the devices happen. Some traditonal forensic methods and techinques that are used for standard digital forensics may be very difficult to apply to IoT forensics. For example, carving (searching for specific content in an extracted file system image) could be difficult as many IoT devices, rely on flash memory and have no built-in filesystem storage capacity. There is a lack of consistency in format that it can be difficult to produce human-readable evidence.  
**Notes:** The paper also includes an example in 2016 of a DoS attack against Dyn domain name servers that occurred from IoT devices. This occurred due to their vulnerabilities being exploited. The attack affected traffic to popular sites such as Twitter, Spotify, and Reddit.  
