# Active Directory Project 2.0

## Objective

The project aims to implement a centralized log monitoring and alerting solution by deploying Splunk on a Ubuntu Server. Logs from both an Active Directory (AD) server and a Windows user machine are forwarded in real-time using Splunk Universal Forwarders, enabling centralized data collection and visibility. This setup forms the foundation for monitoring authentication activity, system events, and potential security incidents across the environment.

To enhance security operations, the project incorporates Shuffle, an open-source SOAR platform, to automate alert analysis and event correlation. Additionally, Slack is integrated as an interactive messaging tool to notify SOC analysts of critical security events and enable prompt responses. Together, these components simulate a real-world Security Operations Center (SOC) workflow, providing automated detection, response, and analyst collaboration for improved incident handling and situational awareness.
### Skills Learned

- Splunk Deployment & Configuration: Installed and configured Splunk on a Linux server, built custom dashboards and alerts.
- Log Forwarding & Parsing: Setup and fine-tuned Splunk forwarders on Windows systems to forward system, security, and AD logs.
- SOAR (Security Orchestration, Automation, and Response): Used Shuffle to create automation workflows for handling alerts.
- Security Event Correlation: Analyzed log data to identify suspicious patterns (e.g., brute force, lateral movement).
- Slack Bot Integration: Used Slack Webhooks or API to push alerts and receive analyst responses.
- Scripting/Automation: Developed automation logic for filtering and responding to log-based triggers.
- Incident Response Workflow Design: Simulated end-to-end detection to response pipeline in a SOC-like environment.

### Tools Used

| Tool / Platform                       | Purpose                                                                 |
| ------------------------------------- | ----------------------------------------------------------------------- |
| **Ubuntu Server**                     | Hosts the Splunk instance (indexer/search head).                        |
| **Splunk Enterprise**                 | Log management, search, visualization, and alerting.                    |
| **Splunk Universal Forwarder**        | Installed on AD server and user machine to collect logs.                |
| **Active Directory (Windows Server)** | Acts as authentication and log source.                                  |
| **Windows User Machine**              | End-user device for log generation (e.g., login attempts, failed auth). |
| **Shuffle (SOAR Platform)**           | Automates playbooks for log analysis, enrichment, and response.         |
| **Slack**                             | Sends automated alerts and allows two-way interaction with SOC team.    |


## Steps
***Playbook Diagram***
![Active Directory Playbook_-Page-2 drawio (1)](https://github.com/user-attachments/assets/12560f73-5ac4-4d93-8ce5-befce04699de)

***Virtual Machines on the Cloud***
![Virtual machines on the cloud](https://github.com/user-attachments/assets/b9182423-316c-4541-a235-d251e779380e)

***Installing Splunk on Ubuntu Server***
![Installing Splunk on Ubuntu Server](https://github.com/user-attachments/assets/043d638c-ccea-4625-8b04-d322397b8175)

***Configuring Active Directory Server***
![Configured Active Directory ](https://github.com/user-attachments/assets/48fa144c-39b3-4164-8f04-e8fe152d6a39)

***Created New AD User***
![New AD User](https://github.com/user-attachments/assets/e97af065-2610-46fd-8e91-39e444612dc6)

***Installing Splunk Universal Forwarder on AD User (as test machine)***
![installing splunk univ  frwd on test machine](https://github.com/user-attachments/assets/aac05189-6bb8-4d64-b5e7-654fee5a115f)

***Splunk Web int.***
![splunk web int](https://github.com/user-attachments/assets/4270dbe4-b11e-4e5b-87fb-064997d9754a)

***installing Splunk universal forwarder on test machine***
![installing splunk univ  frwd on test machine](https://github.com/user-attachments/assets/868c1d9f-6864-4159-9838-beca03584385)

***Modifying input.conf file***
![modifying inpute conf file](https://github.com/user-attachments/assets/175e122d-c02a-4746-9e80-89de3b9d55ee)

***Logs getting ingested to splunk***
![Logs getting ingested to splunk ](https://github.com/user-attachments/assets/d7aa0a5f-b016-4cc7-9ea9-80e0f207ec98)

***Unauthourized Splunk Login Query***
![UnauthourizedSplunkLoginQuery](https://github.com/user-attachments/assets/6d722a1d-7577-490d-ac6d-a411b9dde57b)

***Webhook for Automation***
![Webhook for Automation](https://github.com/user-attachments/assets/b7ec1dc2-45ad-40ab-a265-e9e8f53e5d05)


