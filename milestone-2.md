# Progress Report March 28th, 2019
## Overview
During this phase of our research we reviewed the documented resources found in milestone 1 in greater detail. We specifically examined the data acquisition techniques that various frameworks and procedures employed. We compiled these methodologies and implemented one data acquisition methodology for our project moving forward.

## Outcomes
##### We identified the following difficulties in establishing a IoT framework  
* **Data Extraction:** IoT devices have many different storage methods. They might use a cloud service, or write to a local hub running a service rather than storing data on the actual IoT devices.  Devices also may not include traditional interfaces for gathering data stored on IoT devices. 

* **Chain of Custody:** Keeping a well document Chain of Custody is a vital process during a forensics investigation. However, with the diversity of IoT devices maintaining the documentation to uphold integrity could be difficult.  

* **Evidence Handling:** Digital evidence can be easily modified which could potentially overwrite important data. Traditional digital devices typically only have one location of storage which is not the case in IoT device. The environment of IoT is much more volatile making data extraction more difficult.  

* **Evidence Identification:** Due to the variety of IoT devices and storage processes, identifying the data needed during an investigation can be challenging. Lack of forensic documentation and tools to collect the data once it has been identified can also be a nightmare for investigators.  

* **Project Objectives:** Our project objectives have changed based upon our research. We discovered that many of the existing frameworks for forensics and IoT forensics are very similar to one another. They focus on a few core principles and differences from traditional forensics to IoT forensics. As a result we've decided to focus more on the practical application of IoT forensics with hands on experiments, and shift away from developing our own framework. 

* **Research and Framework Selection:** We examined multiple digital forensics frameworks from over the years and analyzed their applicability to our project. We determined that the Comprehensive and Harmonized framework proposed by Valgarevic and Venter was the most suitable for our needs. We will also refer to ACPO and NIST.  
 
* **Research Methodology:** We examined and selected technical procedures to use and reference as we move into the hands on portion of our project.  We will refer to the processes and procedures presented in the Computer Forensics Technical Procedure Manual (North Carolina State Bureau of Investigation) and the Forensic Examination of Digital Evidence: A Guide for Law Enforcement (US Department of Justice).  

## Hinderances
##### We identified the following hindrances relating to data acquisition  
* **Acquiring Data over many different devices:** Data acquisition for a multitude of IoT devices could require expertise across different digital forensic branches. IoT devices can work off of a set of technologies including wired and wireless communications, remote and local storage, sensors, location tracking, etc. Extracting evidence from various technologies could require expertise in fields such as computer, mobile, and embedded forensics for local storage, network forensics for data over a communication medium, and cloud forensics for remote storage. (Reference from Internet of Things Forensics: The Need, Process Models, and Open Issues).   

* **Chain of Custody:** When acquiring data from IoT devices, it is important for a forensic perspective to pinpoint where exactly the data came from. From conventional computer and digital forensic practices, it is impractical to use the established search and seizure procedures when finding evidence stored in cloud datacenters. It can therefore be seen as impossible to maintain a chain of custody relating to how, when, and where evidence was acquired. (referenced from IoT forensics: Challenges for the IoA era.) 

* **Data Acquisition Tools:** When attempting to acquire data from IoT devices there is a lack of IoT tools in comparison to traditional digital forensics. IoT devices interact with multiple nodes when transferring and storing data which makes make the acquisition process very complex.  (referenced from IoT Forensic: Bridging the Challenges in Digital Forensic and the Internet of Things).  
  
* **Jurisdiction:** Many IoT devices interact with and store data in the cloud. This means data of interest many not necessarily reside in the same state as the device of interest or even the same country. Attempting to get access to the data stored on data centers outside the country may lead to jurisdiction issues and complicate the data acquisition process.   

* **Non-standardization of devices:** There are many IoT devices on the market, and many that serve similar functions but will likely track different data and possibly store the same data in different formats and places. Investigators need to be aware of the each device they examine, what that device tracks, and how it stores that information.  

* **Variety of storage media on devices:** On IoT devices which actually store data on the device the extraction methods may be very difficult. Physical (invasive or non-invasive) extraction of data may be difficult as well. Devices may not be designed to come apart easily, or may require removing a memory chip to extract the data.  


* **No Standard:** Currently, no nationally or globally accepted standard for digital forensics exists. We have guidelines and recommendations in the forms of NIST and ACPO, which are widely accepted, but are not frameworks. Naturally, this lack of standardization impacts the formation of IoT frameworks, which are based on digital forensics frameworks.  
 
* **Volume of Research:** The field of digital forensics has over 20 years of research and documentation to examine. A clear trend we noticed during our research was that the various frameworks we examined seemed to build off predecessors. As a result, general themes for the field appear in most works.  
## Ongoing Risks
|Risk name  | Impact     | Likelihood | Description | Mitigation |
|-----------|------------|------------|-------------|------------|
| Underdeveloped IoT forensic standard (30) | 10 | 3 | IoT forensics is an emerging field, so it may be difficult to find a formally-recognized, tested IoT forensic standard. | The team could examine developing, informal standards or adapt existing digital forensic methodologies. |
| Limited access to forensic applications (14) | 7 | 2 | Access to industry-approved forensic toolkits may be limited due to inadequate funding. | The team can access the UNO Steal labs, which have FTK installed. Access can be scheduled by Dr. Hale for FTK. |
| Loss of data (32) | 8 | 4 | During the course of the project, data could be corrupted or otherwise lost. | The team will implement redundant data storage. Data gathered from research and hands-on experimentation will be stored on flash drives and Google Drive. |
| No formal funding (30) | 3 | 10 | No grant funding for applications or devices will be provided to the team. All expenses will be out of pocket. | Spending will be minimized wherever possible. IoT devices will be provided by team members and digital investigation tools will be primarily open-source, with the exception of FTK. |
| Lack of device documentation (20) | 5 | 4 | IoT devices may not have comprehensive documentation available for public perusal. | The team is working primarily with IoT devices and software that are known to have extensive documentation. | 