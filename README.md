# The-Honeypot

## Overview
This project focuses on simulating the failed brute-force RDP logins on a world map with their location based on cyber attacker's geolocation data collected in the logs and the magnitude of attacks from each location all over the globe. 

It involved deploying a Windows 10 Virtual Machine (VM) on the Microsoft Azure Cloud platform, configuring Firewall to make its ports open for making it discoverable to attackers and using Azure Sentinel SIEM on the cloud platform to make queries from the custom logs. The custom logs are designed to have fields such as longitude, latitude, country, state, sourcehost IP (attacker's IP), destinationhost IP (victim's IP) that are extracted from the Log Analytics workspace with provided raw logs from the Windows 10 Virtual Machine. A customized Powershell script was used from a GitHub resource to run on the Windows VM with the personal API key obtained from https://ipgeolocation.io to get geolocation data of the source machines(attackers).

With the use of world map visualization on the Azure cloud platform, the attempted RDP failed logins with the physical location and magnitude of the cyber attackers was simulated on the world map at regular intervals for several days to collect the data and study the behavior of cyber attacks. Further analysis of the collected data was performed by the group members of this project by discussing and documenting the defense strategies that can be placed to be safe from such events. 


## Documentation

This is a capstone group project that has been documented by group members with Introduction, Method, Results and Discussion in a Research-oriented approach. 
Find the documentation of The-Honeypot at URL

## Results (Output)

The log data that we collected over a period of running our Windows VM is included in this secion in the form of a csv file. This log data was further used in the Microsoft Azure Sentinel Cloud platform to simulate the collected data of cyber attacks on the world map.
Find the output log data results here: 




