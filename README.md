# APPLICATION OVERVIEW 
<------------------------------------------------------------
*This text should remain in the run book even after completion*
 Document following details in this section
•	Application overview
•	Application subsystems and modules
•	A Brief description of Major Application components (3 to 4 lines for each component) and any document related to these components describing them in detail could be embedded if available.
-------------------------------------------------------------->

The Overview of the PPS application areas include classification, underwriting, projected liabilities, ratemaking and pricing. This section, briefly describe each of these areas.

Classification is the analysis of uncertainty of financial loss and fundamental to insurance. On the one hand, classification is the prelude to the underwriting of potential coverage, while on the other hand, risks need to be properly classified and segregated for pricing purposes. Operationally, risk may be viewed from the perspective of the four classes of assets (physical, financial, human, intangible) and their size, type, and location.

Underwriting is the process of selection through which an insurer determines which of the risks offered to it should be accepted, and the conditions and amounts of the accepted risks. The goal of underwriting is to obtain a safe, yet profitable, distribution of risks. Operationally, underwriting determines the risk associated with an applicant and either assigns the appropriate rating class for an insurance policy or declines to offer a policy.

Projected liabilities are future financial obligations that arise because of a claim against the insurance company. The evaluation of projected liabilities is fundamental to the insurance industry.

Ratemaking and pricing refer to the process of establishing rates used in insurance or other risk transfer mechanisms. This process involves a number of considerations including marketing goals, competition and legal restrictions to the extent they affect the estimation of future costs associated with the transfer of risk. Such future costs include claims, claim settlement expenses, operational and administrative expenses, and the cost of capital.

# Business Overview
  <-------------------------------------------------------------
  *This text should remain in the run book even after completion*
•	Provide business overview of the application
•	Business Segments / LSAs using the application
•	Primary business purpose
-------------------------------------------------------------->

Foremost Specialty Lines PPS stands for Policy Processing Systems. These online applications provide Insurances for specialty products such as Mobile Home, Specialty Dwelling and Commercial Mobile Home. Specialty Dwelling and Commercial Mobile Home products are written as single unit policies or multi-unit policies. PPS is a full policy maintenance system that includes New Business, Renewal Business, Endorsement, Cancellation, Reinstatement, Policy/Flex Stops, Claim / Loss and accounting, Online quoting, and Online policy inquiry systems. 

PPS applications offer coverages for three major products, Mobile Home, Specialty Dwelling and Commercial Mobile Home. PPS uses product codes to distinguish the different products it offers. The product codes from 103 through 107 refer to Mobile Home insurance policies. Product code 444 designates a Commercial Mobile Home policy while product code 381 refers to Specialty Dwelling policies. The STAR application is a web based policy system which is designed to interface with many of the daily tasks performed within the PPS Application. EDR (Electronic Document Retrieval) is the facility where the agents can access policy details, complete declaration pages, see the balance due, review renewal notices and more. This makes it easy for agents to self service their policies. The PPS Online Applications developed for Foremost Insurance Corporation are written in CICS, COMPLETE, COBOL, ADABAS, and DB2 for ordering Loss and Credit information.

Now, a new .NET based solution is provided to maintain the entire processing of the Specialty Dwelling product (381) called as DUCKCREEK. All the speciality dwelling policies going forward will be created in DUCKCREEK online and those transactions will be processed through new set of jobs similar to EAGLE environment after the transactions are loaded to DB2 tables from DUCK online using an ETL process. 


# Application Functionality
 _Note : This text should remain in the run book even after completion
* Provide functional overview of the application
* Key functions supported / provided
*	Explain the functionality of the major modules of the application in 3 or 4 lines and any available document can also be embedded._
 

The application deals with the major functionalities given below. 
These functionalities are described in details in section 3.4.
## SNO	Functional Modules
1.	 Policy Processing - FOCUS Batch
2.	 Policy Processing - FOCUS Online (PPPR)
3.	 Policy Processing - Auto FOCUS 
4.	 Policy Processing - PAR Batch
5.	 Policy Processing - EAGLE Batch
6.	 Policy Processing - EAGLE Inquiry(IN00)
7.	 Policy Processing - PAR/NPD Inquiry (K121)
8.	 Policy Processing - NPD Batch
9.	 Policy Processing - FAST (K128)
10. Policy Processing - FAST Batch
11.	Policy Processing - Generic Rating (K138)
12.	Policy Processing - KARS Microfilm Indexing
13.	Policy Processing – Keyfast
14.	Policy Processing – Correspondence
15.	Policy Processing – BIAS
16.	Policy Processing - Credit Scoring/Reporting
17.	Policy Processing - QMS (Muni-Tax Vendor Software)
18.	Policy Processing - Policy transfer Utility
19.	Policy Processing - SDS Message Mover
20.	Policy Processing - Agency Download
21.	Policy Processing - List Management
22.	Policy Processing - Direct Marketing System (DMS)
23.	Policy Processing - Group-1 Software
24.	Policy Processing – CEA
25.	Policy Processing – DUCK batch


# Application Inputs:

Agent has to feed the data through one of the PPS online applications. 

Speciality dwelling policies will be created in DUCK online and the agent will feed the data in DUCK online system.

# Application Outputs:

There are several entities used in PPS Online applications. The relationship of the entities is as follows:
*	 Online transactions related to Mobile Home policies are stored in PAR Master Files which are ADABAS.           
*	 Online transactions related to Specialty Dwelling and Commercial Mobile Home policies are stored in EAGLE Master Files which are ADABAS.           
*	 Predefined and Conditional values are stored in the form of tables using Tablebase software from on-line and batch applications. 
*	All the new speciality dwelling policies are stored in new DB2 tables for which the data is loaded from DUCK online using a ETL tool.  

