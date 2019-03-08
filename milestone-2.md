# Progress Report March 7th 2018
## Overview
During this phase of research, we examined, compared, and contrasted multiple digital forensic frameworks and guidelines. We've provided notes discussing each framework below. Additionally, we've selected one framework that will serve as our baseline to compare against IoT Forensic frameworks. 

## Quick Notes:

1. **Framework for a Digital Forensic Investigation**  
**Authors:** Michael Kohn, Jan Eloff, and Martin Oliver  
**Date Published:** July 5 2006  
**Published In:** ISSA 2006 from Insight to Foresight Conference  
**Proposed Framework:** This framework consists of three stages: Preparation, Investigation, and Presentation. Preparation involves gathering the resources necessary to conduct an investigation, including notifying the relevant authorities and obtaining warrants. The Investigation stage consists of acquiring the devices, conducting an investigation, and analyzing data. The Presentation stage requires investigators to present their findings to the relevant audiences and documenting the investigation.  
**Notes:** Overall, the framework is rather simple. It was designed to not be bogged down by technical details, but to instead remain adaptable. This is one of the oldest frameworks we've examined, so it's a great reference point to demonstrate how far the field has come.  

1. **Systematic Digital Forensic Invesitgation Model**  
**Authors:** Ankit Agarwal, Megha Gupta, Saurabh Gupta, Subhash Gupta  
**Date Published:** January 2011  
**Published In:** International Journal of Computer Science and Security (IJCSS), Volume (5): Issue (1): 2011  
**Proposed Framework:** The Systematic Digital Forensic Invesitgation Model (SDFIM) has 11 cyclical phases: Preparation, Securing the Scene, Survey and Recognition, Documentation of Scene, Communication Shielding, Evidence Collection, Preservation, Examination, Analysis, Presentation, and Review. During the Preparation phase, investigators will gain an initial understanding of the scene and gather the appropriate materials for a forensic investigation. The Securing the Scene phase, investigators lock down the scene. During Survey and Recognition, investigators evaluate the crime scene to determine which devices to capture and analyze; they also conduct intial interviews. Documentation and the chain of custody is initiated in the Documentation of Scene stage. In the Communication Shielding stage, devices are secured in Faraday bags and transported. Volatile and Non-volatile evidence is gathered during the Evidence Collection stage. In the Preservation phase, captured data is stored securely. During the Examination and Analysis phases, data is processed. During the Presentation phase, investigators report their findings to law enforcement and relevant parties. Finally, in the Review phase, investigators review their findings and processes to determine areas of improvement.  
**Notes:** SDFIM is comprehensive, but also cumbersome. It provides several recommendations and elucidates on what events should take place during each step of its execution. This framework is clearly meant to be used by law enforcement agencies to prosecute criminal cases.  

1. **Guide to Integrating Forensics Techniques into Incident Response**  
**Authors:** Karen Kent, Suzanna Chevalier, Tim Grance, and Hung Dang  
**Date Published:** August 2006  
**Published In:**  
**Proposed Framework (summary):** This is to be used as a guide for organizations working to develop their own forensic plan. They express it should be a starting point to help companies, but it should not be used to guide the execution of a digital forensic investigation and that the organization should consult with legal experts as they create their plan. The guide lays out four basic phases for digital forensics: Collection, Examination, Analysis, and Reporting. In the Collection phase the organization should identify, label, record, and acquire data from relevant sources. In the Examination phase, manual and automatic process should be used to extract and assess data of interest while ensuring the integrity of that data. The Analysis phase uses the data gathered to answer questions that lead to the collection of the data (i.e. Did employee X misuse their computer resources?). Lastly, in the Reporting phase the results of the previous phase, actions taken, tools, techniques, and procedures used should be presented and compiled into a final report. This guide is massive and includes sections on forensic staffing, commonly used media types, filesystems, file headers, volatile data, and so on. This report is 121 pages long with a wealth of information to help guide those looking to add forensic capability to their organization.   
**Notes:** This is not a standard or framework, but it may still be useful to reference throughout our paper as it should be used as a starting point for those inducing forensics into their organization. The report itself is highly referenced and one of the more recent publications on this topic from the US government.   

1. **Forensic Examination of Digital Evidence: A Guide for Law Enforcement**  
**Authors:** US Department of Justice  
**Date Published:** April 2004  
**Published In:**   
**Proposed Framework (summary):** This is a guide for law enforcement officials who will be examining digital evidence. The report starts with considerations for the agency (i.e. Is your agency prepared?) and continues to focus more on a step-by-step guide on collecting, examining, and analyzing digital evidence. It also includes case examples to illustrate the process and include a report that might be generated for that case following the procedure. The phases they lay out are: Policy and Procedure Development, Evidence Assessment, Evidence Acquisition, Evidence Examination, and Documenting and Reporting.   
**Notes:** This document targets law enforcement officials but may be useful to show that the procedures laid out for traditional forensics might not work as well with IoT devices. It gives a step-by-step process that officials should take when confronted with digital evidence.   

1. **Computer Forensics Technical Procedure Manual** 
**Authors:** North Carolina State Bureau of Investigation  
**Date Published:** August 25, 2010  
**Published In:**  
**Proposed Framework (summary):** This is similar to the DOJ report, but more detailed. Each section gives a breakdown on what the protocol is, its purpose, equipment needed, term definitions, calibrations needed for tools, limitations, the procedure, references, and notes. This is a step-by-step technical guide meant to be used by law enforcement agencies of North Carolina as they investigate crimes with digital evidence.   
**Notes:** As with the DOJ report, it might be useful to have a more technical step-by-step guide to show how current procedures need to be updated for IoT. This is almost 10 years old now, more recent than the DOJ report, but I do not think the procedures vary too much from what they are today. The report mentions many of the same forensic tools we have heard of from class.   


* [ACPO Good Practice Guide](https://www.digital-detective.net/digital-forensics-documents/ACPO_Good_Practice_Guide_for_Digital_Evidence_v5.pdf)
* [NIST Guide to Integrating Forensic Techniques into Incident Response](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-86.pdf)
* [A Comprehensive and Harmonized Digital Forensic Investigation Process Model](https://onlinelibrary-wiley-com.leo.lib.unomaha.edu/doi/epdf/10.1111/1556-4029.12823)
* [Technical Plan From North Carolina](https://www.ncdoj.gov/about-doj/crime-lab/crime-laboratory-documentation/computer-technical-procedure-manual-8-25-2010.aspx)
* [DOJ Guide for Law Enforcement](https://www.ncjrs.gov/pdffiles1/nij/199408.pdf)
* Digital Forensic Science : Issues, Methods, and Challenges (ebook)
* Handbook of digital forensics of multimedia data and devices (ebook)

## Outcomes
(brief overview of outcomes - what did you achieve?)

also list them out like this:
* Investigate DF frameworks 
  We did this. 
* outcome 2

## Hinderances
(insert brief discussion of challenges encountered)

## Ongoing Risks
(address your project risks identified from Milestone 1 and update them based on your current progress, this should be a table)
