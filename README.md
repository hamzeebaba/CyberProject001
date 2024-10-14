# Network Security Protocol and Attack Analysis

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Conclusions](#conclusions)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

## Project-Overview
This project aims to analyze the most common protocols used in cyber attacks across different network segments and identify the most frequent types of attacks for each network segment. The analysis will provide valuable insights for the network security team and cybersecurity analysts to enhance their defensive strategies and resource allocation.

## Data Sources
Cybersecurity Data : The primary data used for this is the "cybersecurity_attacks.csv" file, containing detailed information about the network and attacks on the network.

## Tools
- Microsoft Excel (for pivot tables and data analysis)

## Data Cleaning/Preparation
In the initial phase, the following was performed
- Data loading and inspection
- Data formating
- Removing duplicate entries
- Handling missing values
- Ensuring consistent naming conventions for network segments]

## Exploratory Data Analysis
Initial exploration of the Data to answer key questions
- What are the most common protocols (e.g., TCP, UDP, ICMP) used in cyber attacks across different network segments?
  
![cyber protocols in cyber attack](https://github.com/user-attachments/assets/ba7fc7bb-1066-43f6-9dfa-cc4121629b7b)

- What types of attacks (based on 'Attack Type' and 'Attack Signature') are most frequent for each network segment (e.g., Segment A, Segment B, etc.)?
  
![Most common cyber attacks in a network segment](https://github.com/user-attachments/assets/1a6c1e94-3c8b-4820-bd81-6978767d35a0)


## Data Analysis
The analysis was conducted in two main parts:

1. Protocol Analysis:
   - Created a pivot table in Excel
   - Used Network Segment as rows, Protocol as columns, and protocol count as values
   - Sorted data to identify the most common protocols for each network segment
  

2. Attack Type Analysis:
   - Created a pivot table in Excel
   - Used Network Segment as rows, and Attack Type/Signature as values
   - Sorted data to identify the most common attack types and signatures for each segment

## Results

1. Protocol Analysis:
   - Segment A: Top protocol in this segment is ICMP (4442)
   - Segment B: Top protocol in this segment is ICMP (4471)
   - Segment C: Top protocol in this segment is ICMP (4516)
  
2. Attack Type Analysis:
   - Segment A: Most common attack are MALWARE (4479)
   - Segment B: Most common attack are INTRUSION (4497)
   - Segment C: Most common attack are DDOS (4517)

## Conclusions

- Different network segments show varying vulnerabilities to specific protocols and attack types.
- ICMP is consistently the most exploited protocol across all segments.
- Most common attack types is DDOS in segment C.

## Recommendations
1. Protocol-based recommendations:
   - Implement stricter firewall rules for high-frequency attack protocols, especially ICMP
   - Allocate additional monitoring resources to network segments with higher-risk protocol profiles

2. Attack type-based recommendations:
   - Develop tailored defensive measures for each network segment based on their most common attack types
   - Prioritize security training and tools that address the most frequent attack signatures in each segment

## Limitations
- The analysis is based on historical data and may not reflect emerging attack trends
- The effectiveness of recommended measures may vary and should be continuously monitored and adjusted
- The analysis does not account for the severity or impact of each attack, only their frequency

## References
- [Youtube](https://www.youtube.com/watch?v=0N9xekdKCwk)
- [Kaggle](https://www.kaggle.com/datasets/teamincribo/cyber-security-attacks)

---

For more information, please contact [Your Name] at [your.email@company.com].
