# Domain 1 : Security and Risk Management
## Agenda 
- Principles of Security
- Security Governance 
	+ Security Strategy
	+ Security Blueprints and Frameworks 
- Information Security Program 
- Information Security Risk Management 
	+ Identification 
	+ Assessment 
	+ Mitigation 
	+ Monitoring 
- Legal Considerations 
- Knowledge Transfer 

## Information Security Program
- Provides the means for achieving strategy 
- Policies/Standards/Procedures/Guidlines
- Roles and Responsibilities 
- SLA's Service level agreements/Outsourcing 
- Data Classification/Security 
- C&A (Certifications and Accreditation)
- Auditing 
  
### Policies 
We start by looking at policies : 
- `Corporate policy (Organizational policy)`: state management commitment to security. 
> Policies dont frequently change, Standards are the ones we change instead, Policies are very broad and generic 
- `System Specifique Policy` : directed at an individual system. Example : "before accessing {domain controllers}, users must provide a multifactor authentication based on the type of access they're to be granted"
- `Issue Specific Policy` : Nebulous issues qithin the organisation we need to define because we cant rely on common sense. Example : 
	+ **Change Management Policy** : we dont just make changes out of the blue. We need processes to implements changes.
	+ **Acceptable Use Policy** : how can you use company ressources. 
	+ **Privacy** : users and employees expect privacy in the workplace, if employers are to infringe up on privacy of employees they must inform them -> most important thing is notification.
	+ **Data/System Ownership** : make sure its clear who owns what in your system, because the system and the data owners are the ones to determine the classifications and dictate the controls.
	+ **Seperation of Duties SOD** : no one individual must have too much power and authority to do too many things, the person that prints the pay-checks isnt the one who signs them. It forces collusion : many people should collude to commit a fraud. 
	+ **Mandatory Vacations** : Detective controls which are implemented at very specific occasions. Example if an employee is suspected for fraud, they can be forced to take mandatory vacations to investigate if they are the ones causing problems.
	+ **Job Rotation** : Detective Control. example : If i am database administrator A and you move me to database administrator B it gives someone else the change to view my work.
	+ **Least Privilege** : About actions - What can you do. "I'll only allow a network admin to access the network remotly". 
	+ **Need to Know** : About Data - You dont need to access the sales folder unless you are in the sales group
	>Both Least privilege and Need to know go hand in hand with Seperation of duties.
	
	+ **Dual Control** :  Preventing abuse of power. "In order to launch a bomb you need two people". "In order to retrieve a key i need both Alex and Diana". 
But what if one of the two isnt present ? then we have: 
	+ **M of N control** : Maybe i have N network administrator, i need M network administrator  to preform a privileged action.

### Standards 
They define the specifics of policies, the details of how thats going to be done.  
While we have few policies that rarely change, we will have many standards that will frequently change. I'll have standars for each users groups, standards that apply to certaint type of informations certain systems. 
they are : 
+ Mandatory 
+ Created to support policy, while providing more specific details
+ Reinforces policy and provides direction 
+ Can be internal or external 

### Procedures 
They are : 
+ Mandatory 
+ Step by step directives on how to accomplish an end-result
+ Detail the "how-to" of meeting the policy, standards and guidelines 

### Guidelines 
They are : 
+ Not mandatory 
+ Best practices 
+ Suggestive in nature
+ Recommended actions and guides to users. 

Example : In order to maintain securoty awareness, we recommend that our employees attend training classes in relation with security whenever possible. 
```
Procedures  : How  
Standards   : What 
Policies    : Why 
```
### Baselines 
+ Mandatory 
+ Minimum acceptable security configuration for a system or process 
+ The purpose of security classification is to determine and assign the necessary baseline configuration to protect the data
+ Can be used for variance analysis : if i am worried that other softwares had been installed in my system, i compare it to the baseline image.

### Roles and Responsibilities 
In small companies we may notice that the lines between roles and responsiiblities get blur, where the security team is the network team because they usually have the same set of skills.  
We want to isolate and seperate roles. 
1. **``Senior Management's responsibilities :``** 
	Senior management is ultimately responsible to : 
	+ Provide oversight 
	+ Provide funding and support 
	+ Ensure testing (and that appropriate results are achieved)
	+ Propritize business functions 
	+ Establish a common vision/strategy/framework for the entreprise 
	+ "sign off" on Policy, BIA (Business impact analysis) and other organizational documents 
2. **``Steering Committee :``**
	+ Oversight of infotmation security program 
	+ Acts as liaison between Management, Business, Information Technology, and Information Security
	+ Assess and incorporate results of the risk assessment activity 
	+ Into the decision-making process 
	+ Ensures all stakeholders interests are addressed 
	+ Oversees compliance activities
3. **``Chief Information Security Officer :``**
	+ Strategic Planning 
	+ Policy Development 
	+ Technology Assessment 
	+ Process Improvement 
	+  Acquisitions 
	+ Capital Planning 
	+ Signs off on the architecture to be implemented 
	+ Security
	+ summary : The CIA triade for information assets 
> Now we move from Senior management down to functional management 
4. **``Information Security Management :``**
	+ Functional Manager, responsible for achieving for determining the "How". 
	+ Play a leading role in introducing an appropriate, structured methodology 
	+ Act as major consultants in support of senior management
5. **``Business Managers :``**
These are our customars, the heads of individual departments, of business units, the owners of the systems, the owners of the informations. They determine the classification of the assets which means they determine who accesses the data. they are the ones accountable for the protection of the assets. 
	+ Responsible for business operations 
	+ Provide direction to ensure security is implemented in such a way as to meet business objectives 
	+ Responsible for security enforcment and direction 
	+ Responsible for day-to-day : 
		+ Monitoring 
		+ Reporting 
		+ Disciplinary actions 
		+ Compliance 
		
6. **``Security Practitioners :``**
	+ Responsible for proper implementation of security requirements in their IT systems. 
	+ Support or use the risk management process to identify and assess new potential risk and implement new security controls as needed to safeguard their IT systems. 
7. **`` Auditors :``**
Trick question : at what point in time does the auditor say enough is enough i need to jump here and fix this problem ?  
Answer is : NEVER! Auditors audit. and thats it.  
Auditors are there for compliance, if want to find out if configuration is according to policy -> you audit, are we in compiance with laws and regulations -> you audit. However if you want to know if it works -> you test. 
> Am i in compliance -> Audit  
Will it work -> Test 

+ Objective Evaluation of controls and policies to ensure that they are being implemented and are effective 
+ If internal auditing is in place, auditors should not report to the head of a business unit, but rather to the Chief Operating Officer or some other entity without direct stake in result 
+ Auditors document and do not modify   

8. **``Security Trainers :``**
Its up to security trainers to create a blameless strategy.   
When people understand why we are trying to do what we are trying to do, they tend to be much more willing to follow the policy. 
	+ Must understand the risk management process 
	+ Develop appropriate training materials 
	+ Conduct security trainings and awareness programs catered to roles within the organization 
	+ Incorporate risk assessment into training programs to educate the end users 
	+ Encourage users to report violations 

## Information Security Risk Management 
Before we start implementing controls we have to get risk management.    
It is the foundation of all security decisions.  

>Information security risk management, or ISRM, is the process of managing risks associated with the use of information technology. It involves identifying, assessing, and treating risks to the confidentiality, integrity, and availability of an organization's assets 

### Risk Definitions 

- ``Assets :`` Anything of value to the company
- ``Vulnerability :``A weakness 
- ``Threat :``Something that could pose loss to all or part of an asset 
- ``Threat Agent :``What carries out the attack 
- ``Exploit :`` An instance of compromise 
- ``Risk :`` The probability of a threat materializing 
- ``Controls :`` Physical, Administrative, and Technical Protections 
	+ Safeguards (Proactive) 
	+ Countermeasure (Reactive)
- ``Total Risk :`` The risk that exists before any control is implemented 
- ``Residual Risk :`` Leftover risk after applying a control 
- ``Secondary Risk :`` When one risk response triggers another risk event 
- ``Incident :`` a risk event that has transpired or materialised

### Risk Identification 
#### Risk Identification Process 
```Mermaid 
graph TD
A[Identify Assets] --> B[Identify Threats]--> C[Identify Existing Controls]-->D[Identify Vulnerabilities]-->E[Identify Consequences]--Feed into-->F(Risk Assessment Process)
```
Sadly github .md files still dont support mermaid graph diagrams so im afraid you wont be able to view my charts :unamused:
#### Methods to Identify Risk 
+ Sources of risk documentation 
+ Audit reports incident reports 
+ Interviews wirh SMEs Public media 
+ Annual reports 
+ Press releases 
+ Vulnerability assessment and penetration tests 
+ Business continuity and disaster recovery plans 
+ Interview and workshops 
+ Threat intelligence services 
> How do we Identify risks ? You open your eyes.   
> anywhere you go you are being aware of current threats of information security, when i see a threat materialized with another organization perhaps in the same industry as me i realise that that risk could happen to me too. I look to incident response reports, what incidents have we had, how did we respond, what are the lessons learned.. There are a million ways, we should do the research. we are liable, we have to do the due diligence and do the research. 
#### Alignment wirh Business Goals and Objectives 
+ The first and most important step for a CISM is to understand the business. Review organizational vision and strategy **FIRST**. 
+ Look beyond IT - Risk is measured by the impact the risl has on the business, not on a particular system
+ In order for risk to be integrated into the enterprise, senior management must be supportive and involved
	+ If management funds and supports the risk management processes we will have what we need to be successful 
	+ Good metrics mean that we have attainable objectives which will help us accomplish our goals 
	+ Good communication and transparency helps is make risk-aware business decisions 
	