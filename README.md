Network Forensics Investigation
Overview
This project documents the analysis of a network capture related to a suspected data exfiltration incident. The objective was to identify indicators of compromise, investigate suspicious network activity, and determine how sensitive information was transferred outside the organization.

The investigation was performed using Wireshark and followed a structured network forensics methodology.

Scenario
A fictitious aerospace company suspected that an employee was leaking confidential information to an external party.

Initial indicators suggested that the employee may have been collaborating with a threat actor planning unauthorized access to company assets.

The task was to analyze captured network traffic, identify suspicious communications, and investigate potential data exfiltration techniques.

Objectives
Analyze network traffic captures (.pcap)
Identify suspicious protocols and communications
Investigate authentication activity
Detect file transfer operations
Analyze potential data exfiltration channels
Document findings and indicators of compromise
Tools Used
Wireshark
Network Traffic Analysis
Protocol Inspection
TCP Stream Analysis
UDP Stream Analysis
Packet Analysis
Key Findings
FTP Authentication
The investigation identified FTP credentials transmitted in cleartext.

Username: ftp

Password: sommar2014

File Transfer Activity
The following file upload operation was identified:

STOR msg.txt
This indicated a successful file transfer to a remote system.

Suspicious Network Activity
Additional analysis revealed a significant volume of UDP traffic on port 31337.

Observations included:

Large outbound data transfers
Chunked JSON-formatted payloads
Encoded hexadecimal data
Characteristics consistent with data exfiltration techniques
Skills Demonstrated
Network Traffic Analysis
Network Forensics
Incident Investigation
Protocol Analysis
Threat Hunting
Digital Forensics
Wireshark Investigation
Security Documentation
Lessons Learned
This project provided practical experience in:

Identifying insecure communication protocols
Investigating authentication events
Following and analyzing network streams
Detecting anomalous network activity
Documenting forensic findings
Applying structured investigative techniques
Author
Joaquin Nicolas Fuenzalida Robledo

IT Security Student

Focused on cybersecurity, network security, incident response, and digital forensics.



