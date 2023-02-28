# The-Honeypot

## Contributors
Sam Noureddini, Neel Patel, Alan Kelly and Diego Hernandez

## Overview
This project focuses on simulating the failed brute-force RDP logins on a world map with their location based on cyber attacker's geolocation data collected in the logs and the magnitude of attacks from each location all over the globe. 

It involved deploying a Windows 10 Virtual Machine (VM) on the Microsoft Azure Cloud platform, configuring Firewall to make its ports open for making it discoverable to attackers and using Azure Sentinel SIEM on the cloud platform to make queries from the custom logs. The custom logs are designed to have fields such as longitude, latitude, country, state, sourcehost IP (attacker's IP), destinationhost IP (victim's IP) that are extracted from the Log Analytics workspace with provided raw logs from the Windows 10 Virtual Machine. A customized Powershell script was used from a GitHub resource to run on the Windows VM with the personal API key obtained from https://ipgeolocation.io to get geolocation data of the source machines(attackers).

With the use of world map visualization on the Azure cloud platform, the attempted RDP failed logins with the physical location and magnitude of the cyber attackers was simulated on the world map at regular intervals for several days to collect the data and study the behavior of cyber attacks. Further analysis of the collected data was performed by the group members of this project by discussing and documenting the defense strategies that can be placed to be safe from such events. 


## Documentation

This is a capstone group project that has been documented by group members with Introduction, Method, Results and Discussion in a Research-oriented approach. 
Find the documentation of The-Honeypot at https://github.com/neelspatel999/The-Honeypot/blob/main/The_Honeypot_A_redteamblueteam-2023-02-22-19-45.docx.pdf
## Results (Output)

The log data that we collected over a period of running our Windows VM is included in this secion in the form of a csv file. This log data was further used in the Microsoft Azure Sentinel Cloud platform to simulate the collected data of cyber attacks on the world map.
Find the output log data results here: https://github.com/neelspatel999/The-Honeypot/blob/main/failed_rdp_with_geo.csv
## References
1. CISA. What is Cybersecurity? | CISA. www.cisa.gov. Published November 14, 2019. https://www.cisa.gov/uscert/ncas/tips/ST04-001
2. Bošnjak, L., Sres, J. & Brumen, B. (2018). Brute-force and dictionary attack on hashed real-world passwords. 1161-1166. doi:https://doi.org/10.23919/MIPRO.2018.8400211 
3.  Grover V. (2020) An Efficient Brute Force Attack Handling Techniques for Server Virtualization. SSRN Electronic Journal. doi:https://doi.org/10.2139/ssrn.3564447
4. Madakor J. (2022) Failed RDP to IP Geolocation Information. GitHub. https://github.com/joshmadakor1/Sentinel-Lab/blob/main/Custom_Security_Log_Exporter.ps1
5. Madakor J. (2021), SIEM Tutorial for Beginners | Azure Sentinel Tutorial MAP with LIVE CYBER ATTACKS! www.youtube.com. Accessed February 24, 2023. https://www.youtube.com/watch?v=RoZeVbbZ0o0&t=1938s
6. Free IP Geolocation API and Accurate IP Geolocation Database. ipgeolocation.io. Published 2021. Accessed February 24, 2023. https://ipgeolocation.io
7. Arntz, P. (2021). RDP abused for ddos attacks: Malwarebytes labs. Malwarebytes. Retrieved February 27, 2023, from https://www.malwarebytes.com/blog/news/2021/01/rdp-abused-for-ddos-attacks

## Acknowlegements
1. Michael Veenstra, Lead Instructor, Fullstack Academy
2. Colin Reyes, Co-Instructor, Fullstack Academy
3. Garbo Loo, Mentor, Fullstack Academy
4. Josh Madakor, Instructor, Software, Content Creator - Youtuber
