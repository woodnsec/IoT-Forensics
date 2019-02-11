# Internet of Things (IoT) Forensics Executive Summary 

###### Insure Group 1 Capstone 2019 

- [Executive Project Summary](#executive-project-summary)
- [Proposed project timeline](#proposed-project-timeline)
- [Project-oriented risk list](#risk-list) 
- [Project Methodology](#project-methodology)
- [Resources/Technology needed](#resources-needed) 
- [First Sprint Plan](#first-sprint-plan) 

## Summary and Merit of Project
1. A problem statement identifying relevant issues related to your bid. The problem statement might also discuss why these issues are a problematic for society, a particular industry/sector/company/agency, or a specific technology(ies).
1. Project goals and objectives in a numbered or bulleted list that you propose to undertake to address the identified problem. Clearly identify what you are doing at a high level with minimal technical detail.
1. The merit of accomplishing the project goals and objectives in terms of how it helps end users, society, or particular industries/sectors/companies/agencies.

Goals:
- Research
- Rec. IoT Forensics standard
- Hands on testing to support rec.
- All this first part becomes our methodology

Merit:
- ubiquity of IoT devices
- IoT is infecting critical industrial sectors
- Having a standard for IoT forensics investigations could improve the quality and integrity of data gleaned during criminal investigations

ideas:
- Research traditional and IoT forensics
- Research the prevalence of IoT devices in industry and education
- Differences and stuff
- Issues with IoT forensics
- Concerns with IoT forensics
- Hands on experimentation 
- Any devices we can get access to

Goals and objectives:

Living in the world of technology, the Internet of Things (IoT) is becoming more and more popular. The rise of IoT devices has shown to bring a new challenge to the field of forensics. Our goal for this project will be to provide a review on the work done and provide hands on testing with devices we own. We will be incorporating any similarities of traditional forensic practices and see how the relate in the world of IoT. 

### Summary 

The Internet of Things (IoT) intersects with every aspect of modern life from industry to agriculture, education to entertainment, and medicine to law enforcement. With the ubiquity of IoT devices, it’s imperative that forensic investigators can reliably gather data and maintain its integrity throughout the course of an investigation. Currently, there exists no defined and accepted standard for IoT Forensic investigations. This can be attributed in part to the heterogeneous nature of IoT. Nearly every class of IoT device integrates its own hardware and software, data storage techniques, and network solutions differently. Even devices from the same category can vary in design and functionality. For example, Google and Amazon both produce home assistants. However, Google Home operates best as an in-house search engine while the Amazon Echo facilitates convenient online shopping. The nature and purpose of the device will also have an effect on the data that can be gathered; wearables and smart appliances will not generate the same types or volume of data. The data these devices gather and generate may be stored locally or on the cloud, compounding the complexity of the data acquisition process.

The creation of a standard is necessary as IoT devices become sources of evidence in criminal, civil, and corporate investigations. Traditional Digital Forensics has been studied extensively and defines standards and procedures that guide investigators in the collection of digital evidence from computers, hard drives, flash drives, and mobile devices. In contrast, IoT Forensics is still an emerging field due in part to the aforementioned reasons. This makes introducing evidence gathered from IoT devices in court difficult as investigators cannot point to best practices and precedent to show their evidence is sound.

### Goals and Objectives

Below we have defined our goals and objectives for this project:  
- Review state of the art research and standards concerning IoT Forensic and traditional digital forensics.  
- Compare and contrast IoT Forensic techniques with those of traditional Digital Forensics standards.  
- Identify the driving factors of the slow maturation of IoT Forensic standards and possible solutions.  
- Apply recommended standards gathered from IoT Forensic literature in hands-on experiments to test their effectiveness across multiple IoT devices.  
- Provide educated recommendations on developing and established IoT Forensic standards, research, and areas that merit further study.

### Merit

Before a standard can be created and implemented, a full understanding of the current field and potential concerns needs to be cultivated. This project will provide a substantive review of the current state of IoT Forensics and examine its differences from traditional Digital Forensics. Our hands-on application of existing methodologies will allow us to formulate recommendations and refinements to the ever-evolving field of IoT Forensics. Additionally, this collection of research can serve as a jumping off point for the creation of an effective IoT Forensic standard.


## Proposed Project Timeline

An important part of project planning is identifying tasks to be completed to address project goals and arranging those tasks in such a way that they can be completed within a (typically) fixed interval of time. In this class, that interval is the length of the semester. For milestone one, prepare an overall project timeline that identifies large tasks to be completed, estimates time of completion, and arranges those tasks chronologically over the project lifespan.
- [ganttpro](https://ganttpro.com) is suggested

[Link to Ganttpro chart](https://app.ganttpro.com/shared/token/aae7d52a7944ba0c0892c645f04c9ce5c976e52f3823376157db230436bf2e7f/394518)

![Alt text](/gantChart.PNG?raw=true "Project Timeline") #TODO upload finished Ganttpro chart from above link. 

## Risk list
As you will probably discover, there are many things that can go wrong when working on a project. Issues with skillsets, technology, team member availability, etc., may arise as the project goes forward. As we discussed in class, there are three options available to deal with project management risks: monitor it (Watch it), mitigate it (do something about it), accept it (give up). For milestone one, you should identify the major sources of risk and what you plan to do about them. Prepare a risk list and rank them by risk level using the standard formula, i.e. `impact x likelihood`, to describe the top 5 risks that might affect your team's ability to pull off the tasks identified in your timeline and dictated by your objectives.

Scale: 1 - 10, 10 being the most impactful / likely 

|Risk name  | Impact     | Likelihood | Description | Mitigation |
|-----------|------------|------------|-------------|------------|
| Underdeveloped IoT forensic standard (30) | 10 | 3 | IoT forensics is an emerging field, so it may be difficult to find a formally-recognized, tested IoT forensic standard. | The team could examine developing, informal standards or adapt existing digital forensic methodologies. |
| Limited access to forensic applications (21) | 7 | 3 | Access to industry-approved forensic toolkits may be limited due to inadequate funding. | The team can access the UNO Steal labs, which have FTK installed. Otherwise, free digital forensic toolkits like SANS SIFT and Autopsy can be procured. |
| Loss of data (32) | 8 | 4 | During the course of the project, data could be corrupted or otherwise lost. | The team will implement redundant data storage. Data gathered from research and hands-on experimentation will be stored on flash drives and Google Drive. |
| No formal funding (30) | 3 | 10 | No grant funding for applications or devices will be provided to the team. All expenses will be out of pocket. | Spending will be minimized wherever possible. IoT devices will be provided by team members and digital investigation tools will be primarily open-source, with the exception of FTK. |
| Lack of device documentation (20) | 5 | 4 | IoT devices may not have comprehensive documentation available for public perusal. | The team is working primarily with IoT devices and software that are known to have extensive documentation. | 

Ideas:
- Maybe not enough information since IOT kinda new and there is a variety of IOT devices nowadays?
- Can't get access to tech
- Can't access applications used for digital forensics
- Unexpected events that delay progress in project
- Loss of data
- Not a lot of research in the field
- Lack of resources (challenge more than risk)
- Two programs for digital forensics (hard to get access to those)
- No funds 


## Project Methodology
Methodology is extremely important for conducting a successful project. While I am always a fan of "winging it" when it comes to day-to-day life - winging it is not an option for being successful on a team. Hence, in this class you will be required to develop a technical plan (AKA `Methodology`) to succeed. Your methodology should be grounded in scientific method and best practice. It should be based on the literature in the area you are working on and should use well-tested methods when possible.

Requirements are extremely important for conducting a successful project - of either the creative or assessment-oriented varieties. Collecting requirements about an application means understand what your end user (or what the end user of a product you are assessing) is going to do with the product. To understand requirements we often define user stories and use cases to encapsulate and represent behavior.

#### Literature Review
For milestone 1, you should prepare a literature review document that surveys the various research and development work in your project area. Your literature review should identify important `keywords`, relevant `research papers`, and `the state of the art` in your area.

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
Once you have examined the relevant literature, you should prepare a technical plan that outlines and defines your methodology. Important consideration should be made to ensure that your methodology uses the literature to the best extent possible. Your technical plan should provide a detailed description of exactly what and how you will do what you plan to do.

## Resources Needed
Every team needs *something* to pull off their project. Clearly identify the technologies and products involved in your project.

Under your requirements section in the README.md file in your GitHub repo, clearly identify the technologies, products, and languages involved in your project. Include a table that identifies which team member will investigate each needed resource. Also include a column indicating whether or not material resources are needed from Dr. Hale.

|Resource  | Dr. Hale needed? | Investigating Team member | Description |
|-------------------|---------|---------------------------|-------------|
| FTK | No | Elisabeth Henderson | Confer with Dr. Grispos to gain access to FTK and the Steal labs. |
| Kali Linux | No | Ronald Ramirez | Research penetration testing tools in a Kali environment that would aid in an IoT forensics investigation. | 
| IoT Devices | No | Nate Wood and Amber Makovicka | Relevant devices include wearables, Google Home, Philip Hue lightbulbs (potential), and Arduino. | 
| Device & Toolkit Documentation | Yes | Ashley Leedom | Gather available documentation for IoT devices and forensic toolkits. | 


## First Sprint Plan
This milestone represents the first step forward in your capstone project. As part of that effort, you need to plan your first real sprint.
This part of the milestone is strictly captured by GitHub Projects (its a `Kanban` board technology like Trello). In your Kanban board, create a board following the structure discussed in class (see Lecture 4). Use this structure to identify the tasks that you will tackle in your first sprint. Put those tasks in the **Sprint To-do** category.


## Teamwork
Lastly, it is important that you realize you are working on a TEAM (except for the few of you that are soloing). I will say now, that your grade is dependent on your participation. I will not allow individuals to sluff off on a team. Your grade is therefore based partly on a *participation factor*. Essentially if you don't participate (and trust me We will know) - you will not get all of the team points on your project grade.
