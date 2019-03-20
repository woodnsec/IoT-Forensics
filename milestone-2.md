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
**Proposed Framework (summary):** This is to be used as a guide for organizations working to develop their own forensic plan. They express it should be a starting point to help companies, but it should not be used to guide the execution of a digital forensic investigation and that the organization should consult with legal experts as they create their plan. The guide lays out four basic phases for digital forensics: Collection, Examination, Analysis, and Reporting. In the Collection phase the organization should identify, label, record, and acquire data from relevant sources. In the Examination phase, manual and automatic process should be used to extract and assess data of interest while ensuring the integrity of that data. The Analysis phase uses the data gathered to answer questions that lead to the collection of the data (i.e. Did employee X misuse their computer resources?). Lastly, in the Reporting phase the results of the previous phase, actions taken, tools, techniques, and procedures used should be presented and compiled into a final report. This guide is massive and includes sections on forensic staffing, commonly used media types, filesystems, file headers, volatile data, and so on. This report is 121 pages long with a wealth of information to help guide those looking to add forensic capability to their organization.   
**Notes:** This is not a standard or framework, but it may still be useful to reference throughout our paper as it should be used as a starting point for those inducing forensics into their organization. The report itself is highly referenced and one of the more recent publications on this topic from the US government.   

1. **Forensic Examination of Digital Evidence: A Guide for Law Enforcement**  
**Authors:** US Department of Justice  
**Date Published:** April 2004    
**Proposed Framework (summary):** This is a guide for law enforcement officials who will be examining digital evidence. The report starts with considerations for the agency (i.e. Is your agency prepared?) and continues to focus more on a step-by-step guide on collecting, examining, and analyzing digital evidence. It also includes case examples to illustrate the process and include a report that might be generated for that case following the procedure. The phases they lay out are: Policy and Procedure Development, Evidence Assessment, Evidence Acquisition, Evidence Examination, and Documenting and Reporting.   
**Notes:** This document targets law enforcement officials but may be useful to show that the procedures laid out for traditional forensics might not work as well with IoT devices. It gives a step-by-step process that officials should take when confronted with digital evidence.   

1. **Computer Forensics Technical Procedure Manual**  
**Authors:** North Carolina State Bureau of Investigation  
**Date Published:** August 25, 2010  
**Proposed Framework (summary):** This is similar to the DOJ report, but more detailed. Each section gives a breakdown on what the protocol is, its purpose, equipment needed, term definitions, calibrations needed for tools, limitations, the procedure, references, and notes. This is a step-by-step technical guide meant to be used by law enforcement agencies of North Carolina as they investigate crimes with digital evidence.   
**Notes:** As with the DOJ report, it might be useful to have a more technical step-by-step guide to show how current procedures need to be updated for IoT. This is almost 10 years old now, more recent than the DOJ report, but I do not think the procedures vary too much from what they are today. The report mentions many of the same forensic tools we have heard of from class.   

1. **A Comprehensive and Harmonized Digital Forensic Investigation Process Model**  
**Authors:** Aleksandar Valgarevic and Hein S. Venter  
**Date Published:** November 2015  
**Published In:** Journal of Forensic Sciences  
**Proposed Framework (summary):** This paper aims at creating a standardized and formalized process of digital forensics. There are five general classes in the model. Readiness processes, an optional process that works to ensure the company is prepared for forensic investigations, should they need to conduct them. Initialization processes, focused on incident detection, first response, and planning for the digital investigation. Acquisitive processes, focused on the physical scene and collecting the digital evidence. Investigative processes,  which focuses on the actual investigation and the tasks that need to be conducted. The last class of processes is the concurrent processes, which the authors describe as novel. These processes should be conducted throughout the entire investigation, such as obtaining authorization, documentation, managing information flow, preserving the chain of custody and so on. Each process class is broken down further into processes and tasks that need to be done. The paper includes a flow chart to show the relationship between these processes and how the output of each process should flow into the input of the next. Some of these processes, such as those in the readiness process class, as iterative so that they can be returned to if needed (i.e. assessment of implementation shows changes are needed, so the company may need to re-define or re-plan their handling of potential digital evidence). The paper gives great detail to each process class and the processes within while also ensuring the model is abstract so it can be fitted as needed.   
**Notes:** This paper gives a very detailed process model for digital investigations. It is written in abstract terms so that it could be applied to many different situations, including IoT. As one of the more recent papers listed, I think it is a good framework to use as a model going forward in our project. In addition, the authors seem to be pushing for standardization using this model, which just adds more weight to the importance of this model.   

1. **ACPO Good Practice Guide for Digital Evidence**  
**Authors:** The Association of Chief Police Officers  
**Date Published:** March 2012  
**Principles (summary):** The ACPO Guidelines consist of four principles that are fundamental to any forensic investigation. The principles are listed below.  
- **Principle 1:** No action taken by law enforcement agencies, persons employed within those agencies or their agents should change data which may subsequently be relied upon in court.  
- **Principle 2:** In circumstances where a person finds it necessary to access original data, that person must be competent to do so and be able to give evidence explaining the relevance and the implications of their actions.  
- **Principle 3:** An audit trail or other record of all processes applied to digital evidence should be created and preserved. An independent third party should be able to examine those processes and achieve the same result.  
- **Principle 4:** The person in charge of the investigation has overall responsibility for ensuring that the law and these principles are adhered to.  
**Notes:** The ACPO Guidelines were adopted by police forces in England, Wales and Northern Ireland. These principles provide guidance for any law enforcement entity that may have to deal with digital evidence. As a result, its recommendations provide an excellent baseline for any forensic framework. We can judge the efficacy of any frameworks we research by analyzing how well they comply with the ACPO guidelines, specifically the principles.  

## Outcomes
##### We have accomplished the following activities:   
 * **Research and Framework Selection:** We examined multiple digital forensics frameworks from over the years and analyzed their applicability to our project. We determined that the Comprehensive and Harmonized framework proposed by Valgarevic and Venter was the most suitable for our needs. We will also refer to ACPO and NIST.  
 
 * **Research Methodology:** We examined and selected technical procedures to use and reference as we move into the hands on portion of our project.  We will refer to the processes and procedures presented in the Computer Forensics Technical Procedure Manual (North Carolina State Bureau of Investigation) and the Forensic Examination of Digital Evidence: A Guide for Law Enforcement (US Department of Justice).  

## Hinderances
##### We have identified the following hinderances:  
 * **No Standard:** Currently, no nationally or globally accepted standard for digital forensics exists. We have guidelines and recommendations in the forms of NIST and ACPO, which are widely accepted, but are not frameworks. Naturally, this lack of standardization impacts the formation of IoT frameworks, which are based on digital forensics frameworks.  
 
 * **Volume of Research:** The field of digital forensics has over 20 years of research and documentation to examine. A clear trend we noticed during our research was that the various frameworks we examined seemed to build off predecessors. As a result, general themes for the field appear in most works.  
