# Analyzing-a-vulnerable-system-for-a-small-business
Small-Business-Vulnerability-Assessment
# **Vulnerability Assessment Report**

## **1st January 20XX**

## ---

# **System Description**

The server hardware consists of a powerful CPU processor and 128GB of memory. It runs on the latest version of Linux operating system and hosts a MySQL database management system. It is configured with a stable network connection using IPv4 addresses and interacts with other servers on the network. Security measures include SSL/TLS encrypted connections.

# **Scope**

The scope of this vulnerability assessment relates to the current access controls of the system. The assessment will cover a period of three months, from June 20XX to August 20XX. [NIST SP 800-30 Rev. 1](https://docs.google.com/document/d/1pRpdpQMEWskxSkwqEMv8W7A7x8GXQlcn0hEcDzWet3Y/template/preview?usp=sharing&resourcekey=0-3GRRWAd8HryVgof-Jc33yA) is used to guide the risk analysis of the information system.

# **Purpose**

Consider the following questions to help you write:

* *How is the database server valuable to the business?*  
  The database server contains huge amounts of data ranging from sensitive PIIs to business operational and user data.  
* *Why is it important for the business to secure the data on the server?*  
  These data business runs and security of the data in the database gives trust to customers.  
* *How might the server impact the business if it were disabled?*  
  Business continuity is lost, trust is broken, recovering business operations might result in financial loss for any operation participants.

# **Risk Assessment**

| Threat source | Threat event | Likelihood | Severity | Risk |
| :---- | :---- | :---- | :---- | :---- |
| *Hacker* | *Obtain sensitive information via exfiltration* | *3* | *3* | *9* |
| *Employee* | *Falling for Phishing, Insider attacks* | *2* | *3* | *6* |
| *Customer* | *Altering Critical information*  | *1* | *3* | *3* |
| *Business partners* | *Access to sensitive or critical information*  | *1* | *2* | *2* |

# **Approach**

Risks considered the data storage and management methods of the business. The likelihood of a threat occurrence and the impact of these potential events were weighed against the risks to day-to-day operational needs.

# **Remediation Strategy**

Implementation of authentication, authorization, and auditing mechanisms to ensure that only authorized users access the database server. This includes using strong passwords, role-based access controls, and multi-factor authentication to limit user privileges. Encryption of data in motion using TLS instead of SSL. IP allow-listing to corporate offices to prevent random users from the internet from connecting to the database.
