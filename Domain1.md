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

## Roles and Responsibilities 
If your ne
