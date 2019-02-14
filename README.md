# Internet of Things (IoT) Forensics Executive Summary 

###### Insure Group 1 Capstone 2019 

- [Executive Project Summary](#executive-project-summary)
- [Proposed project timeline](#proposed-project-timeline)
- [Project-oriented risk list](#risk-list) 
- [Project Methodology](#project-methodology)
- [Resources/Technology needed](#resources-needed) 
- [First Sprint Plan](#first-sprint-plan) 

### Executive Project Summary 

The Internet of Things (IoT) intersects with every aspect of modern life from industry to agriculture, education to entertainment, and medicine to law enforcement. With the ubiquity of IoT devices, it is imperative that forensic investigators can reliably gather data and maintain its integrity throughout the course of an investigation. Currently, there exists no defined and accepted standard for IoT Forensic investigations. This can be attributed in part to the heterogeneous nature of IoT. Nearly every class of IoT device integrates its own hardware and software, data storage techniques, and network solutions differently. Even devices from the same category can vary in design and functionality. For example, Google and Amazon both produce home assistants. However, Google Home operates best as an in-house search engine while the Amazon Echo facilitates convenient online shopping. The nature and purpose of the device will also have an effect on the data that can be gathered; wearables and smart appliances will not generate the same types or volume of data. The data these devices gather and generate may be stored locally or on the cloud, compounding the complexity of the data acquisition process.

The creation of a standard is necessary as IoT devices become sources of evidence in criminal, civil, and corporate investigations. Traditional digital forensics has been studied extensively and defines standards and procedures that guide investigators in the collection of digital evidence from computers, hard drives, flash drives, and mobile devices. In contrast, IoT forensics is still an emerging field due in part to the aforementioned reasons. This makes introducing evidence gathered from IoT devices in court difficult as investigators cannot point to best practices and precedent to show their evidence is sound.

### Goals and Objectives
- Review state of the art research and standards concerning IoT forensic and traditional digital forensics.  
- Compare and contrast IoT forensic techniques with those of traditional digital forensics standards.  
- Identify the driving factors of the slow maturation of IoT forensic standards and possible solutions.  
- Apply recommended standards gathered from IoT forensic literature in hands-on experiments to test their effectiveness across multiple IoT devices.  
- Provide educated recommendations on developing and establishing IoT forensic standards, research, and areas that merit further study.

### Merit

Before a standard can be created and implemented, a full understanding of the current field and potential concerns needs to be cultivated. This project will provide a substantive review of the current state of IoT forensics and examine its differences from traditional digital forensics. Our hands-on application of existing methodologies will allow us to formulate recommendations and refinements to the ever-evolving field of IoT forensics. Additionally, this collection of research can serve as a jumping off point for the creation of an effective IoT forensic standard.


## Proposed Project Timeline
The latest updates on the timeline are available here: [Ganttpro](https://app.ganttpro.com/shared/token/aae7d52a7944ba0c0892c645f04c9ce5c976e52f3823376157db230436bf2e7f/394518) 

![Alt text](/ganttChart_IoT_19.png?raw=true "Project Timeline")

## Risk list
|Risk name  | Impact     | Likelihood | Description | Mitigation |
|-----------|------------|------------|-------------|------------|
| Underdeveloped IoT forensic standard (30) | 10 | 3 | IoT forensics is an emerging field, so it may be difficult to find a formally-recognized, tested IoT forensic standard. | The team could examine developing, informal standards or adapt existing digital forensic methodologies. |
| Limited access to forensic applications (21) | 7 | 3 | Access to industry-approved forensic toolkits may be limited due to inadequate funding. | The team can access the UNO Steal labs, which have FTK installed. Otherwise, free digital forensic toolkits like SANS SIFT and Autopsy can be procured. |
| Loss of data (32) | 8 | 4 | During the course of the project, data could be corrupted or otherwise lost. | The team will implement redundant data storage. Data gathered from research and hands-on experimentation will be stored on flash drives and Google Drive. |
| No formal funding (30) | 3 | 10 | No grant funding for applications or devices will be provided to the team. All expenses will be out of pocket. | Spending will be minimized wherever possible. IoT devices will be provided by team members and digital investigation tools will be primarily open-source, with the exception of FTK. |
| Lack of device documentation (20) | 5 | 4 | IoT devices may not have comprehensive documentation available for public perusal. | The team is working primarily with IoT devices and software that are known to have extensive documentation. | 

## Project Methodology
We will begin our project by conducting a review of the current literature and standards related to IoT forensic data acquisition. Additionally, we will examine traditional digital forensics techniques and compare and contrast them to current IoT forensics standards. The review will provide insight on the current state of IoT forensics and allow us to identify outstanding issues in the field. These issues may include concerns about data integrity and privacy. 

The second half of our project will focus on hands-on experimentation with IoT devices. This will allow us to fully understand the forensic and data acquisition process. Lastly, using the knowledge we gain from the review and hands-on application, we will give our recommendations on standards, research, and refinements to IoT forensics moving forward. 

#### Literature Review
**Keywords:** IoT Forensics, Digital Forensics, Network Forensics, Mobile Forensics, IoT, Privacy, Integrity, Process Model, Investigation Frameworks, IoT Standards, Data Acquisition

1. **A Generic Digital Forensic Investigation Framework for Internet of Things (IoT)**  
**Authors:** Victor R. Kebande and Indrakshi Ray  
**Date Published:** September 26, 2016  
**Published In:** 2016 IEEE 4th International Conference on Future Internet of Things (IoT) and Cloud (FiCloud)  
**Summary:** Kebande and Ray have developed a generic IoT forensic investigation framework that reliably supports digital investigations in IoT-based infrastructures. The framework complies with the ISO/IEC 27043:2015 international standard and provides a promising baseline for IoT forensic investigations.  

1. **Internet of Things Mobility Forensics**  
**Authors:** K M Sabidur Rahman, Matt Bishop, and Albert Holt  
**Date Published:** September 2016  
**Published In:** Information Security Research and Education (INSuRE) Conference, 2016  
**Summary:** K. M. S. Rahman, M. Bishop, and A. Holt examine mobility forensics in the world of IoT. The authors focus on IoT devices in smart homes by conducting research used to create a classification process which can be referenced in other IoT environments.

1. **Internet of Things Forensics: The Need, Process Models, and Open Issues**  
**Authors:** Maxim Chernyshev, Sherali Zeadally, Zubair Baig, and Andrew Woodward  
**Date Published:** June 11, 2018  
**Published in:** IT Professional (Volume: 20, Issue: 3, May/June 2018)  
**Summary:** Maxim Chernyshev, Sherali Zeadally, Zubair Baig, and Andrew Woodward present a high-level overview of the need for IoT forensics, the current models in the field, and the open issues around IoT devices and forensic evidence acquisition. Process models discussed include Forensic-Aware IoT, Next Best Thing triage model, and the Digital Forensic Investigation Framework for IoT.

1. **Forensic analysis for IoT fitness trackers and its application**  
**Authors:** Serim Kang, Soram Kim, and Jongsung Kim  
**Date Published:** December 22, 2018  
**Published in:** Peer-to-Peer Networking and Applications  
**Summary:** Serim Kang, Soram Kim, and Jongsung Kim present their findings from studying the forensic data that may be pulled from the wearable devices Xiaomi Mi Band 2 and Fitbit Alta HR, including how forensic investigators can extract and analyze the data. 

1. **Application-Specific Digital Forensics Investigative Model in Internet of Things (IoT)**  
**Authors:** Tanveer Zia, Peng Liu, Weili Han  
**Date Published:** Aug-Sep 2017  
**Published In:** Proceedings of the 12th International Conference on Availability, Reliability and Security Article No. 55  
**Summary:** This material evaluates the quickly growing field of IoT devices and the difficulties that arise when trying to find forensic evidence among the devices. It looks at three different IoT device: Smart home (Nest Smart Thermostat), Wearables (VitalPatch), and Smart City (Intelligent Traffic Management System or ITMS of Verizon). It explains the type of data transferred to the relevant devices and difficulties in trying to extract the data. For example, the Smart Home device can communicate between itself, a mobile app, and to a cloud. Material from the Wearables section may apply to the hands-on section of our project. 

1. **Security of IoT Sensor Networks**  
**Authors:** Jeffrey Cichonski, Jeffrey Marron, Nelson Hastings  
**Date Published:** February 2019 (draft)  
**Published In:** [NIST website](https://www.nccoe.nist.gov/projects/building-blocks/iot-sensor-security)  
**Summary:** The Internet of Things (IoT) universe is continuously evolving and expanding as new products and technologies are introduced to the marketplace. IoT sensor networks—networks of small devices, or nodes that detect, analyze, and transmit physical data—are a prime example of this ongoing evolution. The National Cybersecurity Center of Excellence (NCCoE) at the National Institute of Standards and Technology (NIST) are partnering to develop a project to protect building management systems' IoT sensor networks.  

1. **IoT Forensics: Challenges For the IoA Era**  
**Authors:** Aine MacDermott, Thar Baker, Qi Shi  
**Date Published:** Feb 26-28 2018  
**Published in:** 2018 9th IFIP International Conference on New Technologies, Mobility and Security (NTMS)  
**Summary:** This paper looks at the different challenges faced when forensically analyzing IoT devices. Challenges include the lack of a forensic framework, potential lack of local storage, processing of large IoT data, among other issues. This research also looks at how Cybercrime and IoT forensics are related. 


#### Technical Plan
**High-Level Project Overview**
- The first step is to gather existing information regarding digital forensic standards, frameworks, methods, etc., and see how they apply to IoT forensics. 
  - Review major themes and takeaways from collected research material.
  - Observe major differences and obstacles that exist in IoT forensics that cannot be translated from digital forensic standards.
  - Identify sources of difficulty in creating standards and frameworks for IoT forensics.
- The second step will be to research 1-2 proposed frameworks for IoT forensics and observe possible solutions. 
  - Determine if we can test the framework in our environment(s) with our device(s).
  - Evaluate utility and practicality of the proposed frameworks.
  - Examine limitations and restrictions of the frameworks. 
  - Compare and contrast with traditional digital forensic frameworks.
- The third step is to derive hypotheses about data acquisition from our IoT devices. 
  - What data do we expect to retrieve?
  - What data might we want to retrieve?
  - How difficult will it be to retrieve the desired information?
- The fourth step is to apply the aforementioned frameworks and standards to our IoT devices.
  - Available devices include a Google Mini and wearables.
  - Document individual findings from each device, framework, and standard.
  - Compare the findings with expected results.
- The fifth step is to gather all our documentation and other relevant material from previous experiments and establish an educated conclusion. 
  - Do the proposed frameworks and standards show promise? 
  - How easy/difficult was the process? 
- Finally, the last step is to provide any recommendations in terms of further research, standards, and other considerations in the future.
  - Where can we go from here?
  - Consider any new developments for IoT devices in the future. 
  - Consider what other types of devices could be developed in the near future.

## Resources Needed
|Resource  | Dr. Hale needed? | Investigating Team member | Description |
|-------------------|---------|---------------------------|-------------|
| Forensic Tools| No | Elisabeth Henderson | Confer with Dr. Grispos to gain access to FTK and the Steal labs. |
| Penetration Testing Tools | No | Ronald Ramirez | Research penetration testing tools in a Kali environment that would aid in an IoT forensics investigation. | 
| IoT Devices | No | Nate Wood and Amber Makovicka | Relevant devices include wearables and Google Home Mini.| 
| Device & Toolkit Documentation | Yes | Ashley Leedom | Gather available documentation for IoT devices and forensic toolkits. | 
