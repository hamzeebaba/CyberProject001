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

Company A established in 2012, is a leading global technology company specializing in cybersecurity solutions. The company provides services to a diverse range of clients across various industries, ensuring the security and efficiency of their network operations.

In recent years, Company A has observed a significant increase in the frequency of cyber attacks targeting its clients' networks. This has led to a growing concern about the effectiveness of current security measures and the need for a more data-driven approach to network defense strategies.

The company has gathered substantial amounts of data on cyber attacks, including information on attack vectors, protocols used, affected network segments, and attack types. However, this valuable data has been previously underutilized in formulating defense strategies.

This project aims to analyze this data to uncover critical insights that will enhance Company's A cybersecurity offerings and improve clients' overall network security posture.

Insights and recommendations are provided on the following key areas:

- Protocol Usage Analysis: Evaluation of the most common protocols (e.g., TCP, UDP, ICMP) used in cyber attacks across different network segments.
- Network Segment Vulnerability: Assessment of which network segments are most frequently targeted and through which protocols.
- Attack Pattern Identification: Analysis of recurring attack patterns and their correlation with specific protocols and network segments.
- Attack types: Identify the most common attacks used in each network segment.
- Defense Strategy Optimization: Recommendations for tailored firewall rules and resource allocation based on identified high-risk protocols and segments.

The project utilizes data analysis techniques, including pivot table analysis in Excel, to process and interpret the vast amount of security data collected. This approach allows for a granular examination of attack patterns, attack types and provides a solid foundation for developing more robust and targeted security measures.

By leveraging these insights, Company A aims to significantly enhance its ability to protect clients' networks.

## Data Structure Overview

![image](https://github.com/user-attachments/assets/a800e4c0-d8ed-4b2a-bc15-dd0aca3d14e2)


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
