# Progress Report March 28th, 2019
**Capstone:** IoT Forensics  
**University:** University of Nebraska at Omaha  
**Members:** Elisabeth Henderson, Ashley Leedom, Amber Makovicka, Ronald Ramirez, & Nathan Wood   

- [Overview](#overview)
- [Outcomes](#outcomes)
- [Hinderances](#hinderances) 
- [Ongoing Risks](#ongoing-risks)


## Overview  
The primary concerns of Milestone 2 were digesting the literature discovered in Milestone 1 and furthering our research base. We chose to focus our efforts in three categories: digital forensic frameworks, difficulties in establishing IoT forensic frameworks, and IoT data acquisition. Research in each of these categories furthered our project in several ways.  

IoT forensics draws considerable inspiration and direction from existing digital forensic frameworks and guidelines. As a result, studying existing digital forensic frameworks gives us insight into how an IoT forensic framework could be constructed and, more importantly, the underlying principles these frameworks are meant to encompass. During this phase of our research, we examined multiple digital forensic frameworks from over the last 20 years. We noticed that newer frameworks tended to build and expand upon previous ones, creating more comprehensive frameworks as years persist. Our research culminated in selecting *A Comprehensive and Harmonized Digital Forensic Investigation Process Model* as our de facto digital forensic framework. We will compare IoT forensic frameworks against this model to evaluate their efficacy.    

Currently no standardized IoT forensic framework exists. The research conducted during this phase of the project sought to understand the barriers to creating a standard. This is an issue that stems from many complications. These complications include the wide variety of IoT devices, each with their own uses, makes, models, operating systems, and storage capabilities. Additionally, many of these devices do not store their data locally, but rather offload the data to the cloud which adds another level of complexity to creating a standard. As a standard is meant to be applicable to all of these devices, this variety makes generalizations that are inherent to a standard impossible.  

The last aspect of this Milestone was focused on preparing for the hands-on data acquisition that we will do on our own IoT devices. We have identified common pitfalls that we or others, such as forensics investigators, may fall into when attempting to acquire data from IoT devices. We also outline our approach for the next section and the acquisition methods we plan on using.  

## Outcomes
Our project objectives have changed based upon our research. We discovered that many of the existing frameworks for forensics and IoT forensics are very similar to one another. They focus on a few core principles and differences from traditional forensics to IoT forensics. As a result we've decided to focus more on the practical application of IoT forensics with hands on experiments, and shift away from developing our own framework.  
<br>
#### These are the outcomes we derived after researching digital forensic frameworks  
* **Research Methodology:** We examined and selected technical procedures to use and reference as we move into the hands-on portion of our project.  We will refer to the processes and procedures presented in the Computer Forensics Technical Procedure Manual (North Carolina State Bureau of Investigation) and the Forensic Examination of Digital Evidence: A Guide for Law Enforcement (US Department of Justice).  

* **Research and Framework Selection:** We examined multiple digital forensics frameworks from over the years and analyzed their applicability to our project. We determined that the Comprehensive and Harmonized framework proposed by Valgarevic and Venter was the most suitable for our needs. We will also refer to ACPO and NIST. 

The diagram below details the process flow of the Comprehensive and Harmonized framework.  

![CAHDF](https://user-images.githubusercontent.com/47015888/55125008-502f2080-50d6-11e9-9637-223187b46653.png)  

Concurrent Processes include obtaining authorization, documentation, managing information flow, preserving chain of custody, preserving digital evidence, and interaction with the physical investigation.  

The readiness class is an optional set of processes that are mostly concerned with prepping an organization for an investigation.  

The initialization class deals with the commencement of an investigation and encompasses incident detection, first response, planning, and preparation.  

The acquisitive class is primarily concerned with the collection, transportation, and storage of digital evidence. Investigators must take care to maintain the integrity of all data collected during this stage of an investigation.  

The investigative class is where collected evidence is analyzed, interpreted, and presented to the relevant parties. After a report has been generated and the findings delivered, the investigation is wrapped up and closed.  Evidence is preserved in the event that the investigation must be reopened.  
<br>
#### We identified the following difficulties in establishing an IoT framework standard  
* **Data Extraction:** IoT devices have many different storage methods. They might use a cloud service or write to a local hub running a service rather than storing data on the actual IoT devices.  Devices also may not include traditional interfaces for gathering data stored on IoT devices. 

* **Chain of Custody:** Keeping a well document Chain of Custody is a vital process during a forensics investigation. However, with the diversity of IoT devices maintaining the documentation to uphold integrity could be difficult.  

* **Evidence Handling:** Digital evidence can be easily modified which could potentially overwrite important data. Traditional digital devices typically only have one location of storage which is not the case in IoT device. The environment of IoT is much more volatile making data extraction more difficult.  

* **Evidence Identification:** Due to the variety of IoT devices and storage processes, identifying the data needed during an investigation can be challenging. Lack of forensic documentation and tools to collect the data once it has been identified can also be a nightmare for investigators.
<br>

#### This is the outcome we derived from researching IoT data acquisition techniques  
* **Data Acquisition Plan:** We have identified four data acquisition techniques we would like to attempt on our own devices. These include using FTK to attempt data extraction, hardware-based data extraction, Bluetooth-based data extraction, and acquiring application data from a mobile device.  

## Hinderances
#### We identified the following hindrances relating to the project and conducted research  
* **Acquiring Data over many different devices:** Data acquisition for a multitude of IoT devices could require expertise across different digital forensic branches. IoT devices can work off of a set of technologies including wired and wireless communications, remote and local storage, sensors, location tracking, etc. Extracting evidence from various technologies could require expertise in fields such as computer, mobile, and embedded forensics for local storage, network forensics for data over a communication medium, and cloud forensics for remote storage.   

* **Chain of Custody:** When acquiring data from IoT devices, it is important for a forensic perspective to pinpoint where exactly the data came from. From conventional computer and digital forensic practices, it is impractical to use the established search and seizure procedures when finding evidence stored in cloud datacenters. It can therefore be seen as more difficult and complex to maintain a chain of custody relating to how, when, and where evidence was acquired. 

* **Data Acquisition Tools:** When attempting to acquire data from IoT devices there is a lack of IoT tools in comparison to traditional digital forensics. IoT devices interact with multiple nodes when transferring and storing data which makes make the acquisition process very complex.   
  
* **Jurisdiction:** Many IoT devices interact with and store data in the cloud. This means data of interest many not necessarily reside in the same state as the device of interest or even the same country. Attempting to get access to the data stored on data centers outside the country may lead to jurisdiction issues and complicate the data acquisition process.   

* **Non-standardization of devices:** There are many IoT devices on the market, and many that serve similar functions but will likely track different data and possibly store the same data in different formats and places. Investigators need to be aware of each device they examine, what that device tracks, and how it stores that information.  

* **Variety of storage media on devices:** On IoT devices which actually store data on the device the extraction methods may be very difficult. Physical (invasive or non-invasive) extraction of data may be difficult as well. Devices may not be designed to come apart easily or may require removing a memory chip to extract the data.  

* **No Standard:** Currently, no nationally or globally accepted standard for digital forensics exists. We have guidelines and recommendations in the forms of NIST and ACPO, which are widely accepted, but are not frameworks. Naturally, this lack of standardization impacts the formation of IoT frameworks, which are based on digital forensics frameworks.  
 
* **Volume of Research:** The field of digital forensics has over 20 years of research and documentation to examine. A clear trend we noticed during our research was that the various frameworks we examined seemed to build off predecessors. As a result, general themes for the field appear in most works.  

## Ongoing Risks
|Risk name  | Impact     | Likelihood | Description | Mitigation |
|-----------|------------|------------|-------------|------------|
| Underdeveloped IoT forensic standard (30) | 10 | 3 | IoT forensics is an emerging field, so it may be difficult to find a formally-recognized, tested IoT forensic standard. | The team could examine developing, informal standards or adapt existing digital forensic methodologies. |
| Limited access to forensic applications (14) | 7 | 2 | Access to industry-approved forensic toolkits may be limited due to inadequate funding. | The team can access the UNO Steal labs, which have FTK installed. |
| Loss of data (32) | 8 | 4 | During the course of the project, data could be corrupted or otherwise lost. | The team will implement redundant data storage. Data gathered from research and hands-on experimentation will be stored on flash drives and Google Drive. |
| No formal funding (30) | 3 | 10 | No grant funding for applications or devices will be provided to the team. All expenses will be out of pocket. | Spending will be minimized wherever possible. IoT devices will be provided by team members and digital investigation tools will be primarily open-source, with the exception of FTK. |
| Lack of device documentation (20) | 5 | 4 | IoT devices may not have comprehensive documentation available for public perusal. | The team is working primarily with IoT devices and software that are known to have extensive documentation. | 
