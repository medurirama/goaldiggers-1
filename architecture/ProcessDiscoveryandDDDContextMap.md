[<-- Back to Home](../README.md)

# Process Discovery And DDD Context Map
## Table of Content
1. [Overview](#1_Overview) 
2. [Actors and Definitions](#2_ActorsandDefinitions) 
3. [Core Domains](#3_CoreDomains) 
4. [Supporting Domains](#4_SupportingDomains)
5. [Generic Domains](#5_GenericDomains) 

##  Overview <a name="1_Overview"></a>
As part of the Domain discovery sessions, we have analyzed Spotlight Platform business domains and adopted **Domain Driven Design methodology**. As part of this analysis we have identified different **subdomains**. 

Each **subdomain** resembles a set of interrelated, coherent use cases. These are defined based on the business domain and their functional requirements. In the discovery session the team has analyzed all the functional requirements to identify these subdomains.

## Actors and Definitions <a name="2_ActorsandDefinitions"></a>
![Actors and Definitions](..//Images/ActorsandDefinitions.jpg)

## Core Domains <a name="3_CoreDomains"></a>
The main offering of the Spotlight Platform is **onboarding the Non Profit Community and Candidates**. Once the onboarding activity is completed, the Non-Profit community will be tagged to the Candidate to avail the Service offerings to achieve the career aspirations. <br />
![Core Domains](..//Images/CoreDomains.jpg)

- **Domain: Spotlight Platform** <br />
The Spotlight Platform is a sustained effort to amass a coalition of nonprofits in order to address specific needs within the communities we serve by leveraging a centralized platform as the base of operations to collaborate and make a collective impact.

**Primarily the scope is divided into two areas. Candidate and Non-Profit community**. <br />
So below are the Core Subdomains identified

- **Candidate Onboarding Community**
      - Candidate Registers
      - Undergoes assessment
      - Roadmap gets assigned by the Mentor etc.,
      
- **Non Profit Community**
      - NPC Registers
      - Undergoes assessment
      - Roadmap gets assigned by the Community Leader etc.,
- **Candidate and Non-Profit Community Matching**
      - The main competitive advantage is the Matching Engine. 
      - Based on the candidate’s aspiration, assessment results and the introductory meeting will be held with the community leader
      - The platform should be able to recommend or facilitate the Non Profit Community services to the candidate.
- **NPC Networking HUB**
      - This is a Core Subdomain which should incentivize engagement of the NPC
      - This platform will be the networking hub for the NPC with a dependency on NP Community Domain.
      - For now primarily it is focused on United States but later based on the expansion plans of the Spotlight platform the capacity planning will have to change. 

## Supporting Domains <a name="4_SupportingDomains"></a>
The core intent of the Supporting Domain is to cater the needs of the Core Domains by leveraging the components identified in the Generic domain. 

![Supporting Domains](..//Images/SupportingDomains.jpg)

Below are the **Supporting Domains** identified.

**Platform Management**
- **Administrator** of the Spotlight platform manages the **primary data management**
- Has the complete Administrative control over the platform.
- Provides the primary data needed to the **Status Management Domain.**
- Uploads all the Primary data needed for the Candidate and NPC assessment.
- It has an interface to approve the Candidate Assessments and NPC Assessments posted by the NPC/Candidate Assessment Supporting Domains. 
- **Community Leaders** add the Service Offerings, and it gets into the approval process. Part of the primary data.
- **Mentors** add the Program Offerings, and it gets into the approval process. Part of the primary data.
- Once the NPC get’s approved the Program/Service Offerings get auto populated. Platform Management pre-populates this data to be selected based on the service offerings.
- Primary data to track the Milestones for both Candidate and NPC are managed.

**Note: As the parameters used to assess the Candidate and Non Profit community are different so we have two different subdomains to avoid the dependencies.**

**NPC Assessment Module**
- It creates/evaluates the assessments needed for the Non-Profit Community.
- Assessment has set of questions based on the service capabilities which the NPC is going to offer to the candidates.
- Administrator or the Community Leader can create these assessments, based on the role who has created the assessment undergoes the approval process.
- Integrated with Platform module to get the necessary primary data.

**Candidate Assessment Module**
- It creates/evaluates the assessments needed for a Candidate.
- Assessment has set of questions based on the candidate capabilities/Career aspirations.
- Administrator or the Mentor can create these assessments, based on the role who has created the assessment undergoes the approval process.
- Integrated with Platform module to get the necessary primary data.

**Note: As the parameters used to track the roadmap of the Candidate and Non Profit community are different so we have two different subdomains to avoid the dependencies.**

**NPC Roadmap Tracker**
- It is the primary tracker for the NPC, which is maintained by the **Community Leader.**
- All the **milestones** are captured
- Each milestone will be captured. This domain uses the capabilities of the **Status Management Subdomain. **
- **Performance Measurement**
- Data is provided to **NPC Metrics Management subdomain** to measure the NPC performance.

**Candidate Roadmap Tracker**
- It is the primary tracker for the **candidate**, which is maintained by the Mentor.
- All the milestones are captured, and each milestone will undergo status management. This domain uses the capabilities of the **Status Management Subdomain. ** 
- **Performance Measurement**
- Data is provided to **Candidate Metrics Management subdomain to measure the Candidate performance.**

**Note: As the parameters used to measure the performance metrics of the Candidate and Non Profit community are different we have two different subdomains to avoid the dependencies.**

**NPC Metrics Tracker**
- It is the **primary tracker for the NPC**, which is maintained by the Community Leader.
- All the cadence meetings, touchpoints, general parameters to measure the NPC are all captured in the domain. **This domain uses the capabilities of the Status Management Subdomain.** 
- It also gets data from the **NPC Roadmap Tracker and same gets used for the NPC Performance.**

**Candidate Metrics Management**
- It is the primary tracker of the **candidate, which is maintained by the Mentor.**
- All the **cadence meetings, touchpoints, general parameters to measure the NPC are all captured in the domain. This domain uses the capabilities of the Status Management Subdomain.** 
- It also gets data from the **Candidate Roadmap Tracker and same gets used for the Candidate performance.**
- **Gets primary data from Platform Management to derive the metrics to measure the Candidate.**

**Status Management**
- It’s a supporting domain which provides the status for both the candidate and NPC.

**Reporting**
- View Statistics/Analytics
-	Operational Reports
-	Decision Engine
-	It holds the primary data to manage the workflow of the Candidate and **NPC registration process.**
	It has analytics to provide recommendations for the **Candidate and NPC based on their interests.**
	
## Generic Domains <a name="5_GenericDomains"></a>
The core crux of the Generic Domain is to support the need of the Core and Supporting Domains. Below are the Generic Domains identified. <br />


![Generic Domains](..//Images/GenericDomains.jpg)

[<-- Back to Home](../README.md)

