# SIEM 

## Objective

The Detection Lab project aimed to establish a controlled environment for simulating and detecting logs coming from a controlled Kali VM. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system to identify event alerts of nmap scans. This hands-on experience was designed to deepen my understanding of network security, elastic, and event log in

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate logs into a SIEM by creating Alerts.
- Enhanced knowledge of SIEM detection and VM machine utilization.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis. Elastic Security
- Network analysis tools (such as nmap) for capturing and examining network traffic.
- Kali Linux VM
- Elastic Defend

## Steps

*Step 1 - Setting up Elastic account*

This step is a pre-SIEM setup. To use and analyze logs I've utilized a common application "Elastic" that enables a diverse of options and rules to be used in a log analysis scenario

*Step 2 - Setting up Kali VM*

This is a pre-SIEM setup. To create the Nmap scans and generate a targeting machine that Elastic will be used to analyze logs, I've used Kali Linux a widely used OS that has a diversity of hacking tools (including Nmap). To set up I've used VMWare that simulates a real OS inside a Virtual Machine.

*Step 3 - Setting up agents to collect logs*

After setting up all the prerequisites, I used the Elastic Defend system that required installation in the host (Kali Linux VM). To check if the agent was downloaded correctly I have used the command: sudo systemctl status elastic-agent.service

*Step 4 - Generating security events with Nmap scan*

For this part of the project I just needed some actual logs to be analyzed. Since my goal was to analyze any logs correlated on the Kali machine using Nmap scan I have used commands for it (As shown in the image below)

![Screenshot 2024-08-04 103949](https://github.com/user-attachments/assets/89665a6d-d060-4f9e-8cc8-01b440b2b722)

*Step 5 - Creating a dashboard to visualize events*

For visualization purposes, I have created a dashboard that consists of @timestamp for Horizontal axes & logs counts for Vertical axes to be able to detect the number of logs coming from the Host machine

![Screenshot 2024-08-04 094905](https://github.com/user-attachments/assets/31490563-c0f4-47b0-a46b-299a122705e5)

*Step 6 - Creating an alert rule for Nmap scan events*

I was able to also create a rule alert that not only detects a general point of view of the logs but also specifies and alerts if any Nmap scan was used within the target machine

![Screenshot 2024-08-04 101414](https://github.com/user-attachments/assets/2f0f019c-7bf5-4371-bf95-33ec61ee1c82)

*Step 7 - Analysing Data with events*

After all steps, I have successfully created a basic SIEM to detect and alert any Nmap scans in the host machine

![Screenshot 2024-08-04 102725](https://github.com/user-attachments/assets/820c51b1-6ae8-48f4-9d13-e6f418522b28)

### Conclusion

The Detection Lab project successfully achieved its objective of establishing a controlled environment to simulate and detect logs from a Kali VM, using a SIEM system to identify event alerts of nmap scans. Through this project, I have significantly enhanced my understanding of network security, log analysis, and SIEM functionalities.

## Key Takeaways

*Advanced SIEM Knowledge:* The project provided a deep dive into the practical application of SIEM systems, allowing me to understand the intricacies of log ingestion, analysis, and alert creation.

*Proficient Log Analysis:* I gained the ability to effectively analyze and interpret network logs, identifying key patterns and anomalies that indicate potential security threats.

*Enhanced Technical Skills:* Setting up and configuring tools such as Elastic Security, Kali Linux VM, and Elastic Defend, has improved my technical proficiency and problem-solving abilities in cybersecurity.

*Practical Application of Tools:* Using tools like nmap for generating security events and creating a visual dashboard for event analysis highlighted the practical aspects of network traffic examination and security event monitoring.

## Future Directions

Building on this project, there are several avenues for further exploration:

*Enhanced Detection Capabilities:* Implementing more sophisticated detection rules and leveraging machine learning algorithms to identify complex threats.

*Broader Log Sources:* Expanding the scope of log sources to include a wider variety of network and endpoint devices, providing a more comprehensive security monitoring solution.

*Incident Response:* Integrating incident response procedures within the SIEM system to automate and streamline the response to detected threats.

*Continuous Improvement:* Regularly updating and refining detection rules and alert thresholds to adapt to evolving security landscapes and emerging threats.


## Final Thoughts

This hands-on project has been invaluable in solidifying my understanding of SIEM systems and their critical role in cybersecurity. The skills and knowledge gained will serve as a strong foundation for future endeavors in the field of cybersecurity, enabling me to contribute effectively to the detection and mitigation of security threats. Through continuous learning and practical application, I aim to stay ahead in the ever-evolving domain of cybersecurity.


