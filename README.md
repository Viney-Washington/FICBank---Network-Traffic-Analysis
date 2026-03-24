# FICBank---Network-Traffic-Analysis

Analyzed network traffic using Wireshark to classify protocols (HTTP, TCP, TLS, ICMP), interpret PCAP data, identify unusual traffic patterns, and assess web application risk using OWASP methodology.

[View Project File](https://github.com/Viney-Washington/FICBank---Network-Traffic-Analysis/blob/main/Viney%20Washington%20_Part%20A%20-Analysing%20Network%20Traffic.pdf)

## Project Overview
This project focused on analyzing packet capture (PCAP) data using Wireshark to understand network communication, classify protocols, and identify both normal and unusual traffic patterns within the FIC Bank environment.

## Key Analysis Performed
- Examined TCP packet behavior including sequence numbers, acknowledgment values, and connection termination using RST/ACK flags  
- Identified HTTP traffic over port 80 and interpreted web browsing activity between internal and external systems  
- Classified protocols including HTTP (application layer) and TCP (transport layer) and explained how they work together in client-server communication  

## Network Services and Applications Identified
- **Network Services:**
  - Web communication service (HTTP requests and responses)
  - Reliable transport service (TCP connection management and delivery)  

- **Applications:**
  - Web browser (client generating HTTP GET requests)
  - Web server (responding with requested resources)  

## Traffic Analysis and Monitoring
- Captured and analyzed TLS encrypted traffic during YouTube streaming sessions  
- Identified sustained encrypted traffic patterns indicating media streaming rather than normal browsing  
- Captured ICMP traffic to analyze network diagnostics and host communication (ping requests/replies)  
- Used Wireshark filters (TLS, ICMP) to isolate and analyze specific traffic types  

## Unusual Traffic and Security Findings
- Identified long-duration TLS encrypted sessions to external servers as potential policy violations (non-business streaming traffic)  
- Analyzed ICMP traffic patterns and recognized how repeated ping activity could indicate reconnaissance behavior  
- Evaluated TCP session behavior to differentiate between normal communication and potential malicious activity  

## Risk Assessment (OWASP Methodology)
- Assessed web application risk based on likelihood and impact  
- Classified:
  - Online banking login → **Critical Risk**
  - Internal dashboard → **High Risk**
  - Customer support portal → **Medium Risk**
  - Public website → **Medium Risk**  

## Outcome
Developed a deeper understanding of network protocols, traffic behavior, and security risks by analyzing real packet data. This project demonstrates the ability to interpret network activity, identify potential policy violations, and apply risk-based security analysis in a financial environment.
