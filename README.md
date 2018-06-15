# brane
Crypto-portfolio management tool

# Software Requirements Specification
Version 0.1
Prepared by roshii
2018-06-15
  
Table of Contents
=================
  * [Revision History](#revision-history)
  * [Introduction](#1-introduction)
  * [Overall Description](#overall-description)
    * 2.1 [Product Perspective](#21-product-perspective)
    * 2.2 [Product Functions](#22-product-functions)
    * 2.3 [User Classes and Characteristics](#23-user-classes-and-characteristics)
    * 2.4 [Operating Environment](#24-operating-environment)
    * 2.5 [Design and Implementation Constraints](#25-design-and-implementation-constraints)
    * 2.6 [User Documentation](#26-user-documentation)
    * 2.7 [Assumptions and Dependencies](#27-assumptions-and-dependencies)
  * [External Interface Requirements](#external-interface-requirements)
  * [System Features](#system-features)
  * [Other Nonfunctional Requirements](#other-nonfunctional-requirements)
    * 5.1 [Performance Requirements](#51-performance-requirements)
    * 5.2 [Safety Requirements](#52-safety-requirements)
    * 5.3 [Security Requirements](#53-security-requirements)
    * 5.4 [Software Quality Attributes](#54-software-quality-attributes)
    * 5.5 [Business Rules](#55-business-rules)
  * [Other Requirements](#other-requirements)
* [Appendix A: Glossary](#appendix-a-glossary)
* [Appendix B: Analysis Models](#appendix-b-analysis-models)
* [Appendix C: To Be Determined List](#appendix-c-to-be-determined-list)




## Revision History
| Name | Date    | Reason For Changes  | Version   |
| ---- | ------- | ------------------- | --------- |
| roshii | 2018-06-14 | Initial release | 0.1      |
| roshii | 2018-06-15 | Removed template text, Added feature description, Style correction | 0.1 | 
|      |         |                     |           |

## 1. Introduction
### 1.1 Purpose 
This document describes requirements for a crypto-asset portfolio management tool: brane.  
### 1.2 Document Conventions
TBD
### 1.3 Intended Audience and Reading Suggestions
This document is is intended for developper who would like to contribute to this project and potential users who might need such tool and request features. 
### 1.4 Product Scope
Brane is purposed to ease tracking, reporting and management of crypto-assests held at different exchanges and wallets.
### 1.5 References
TBD

## Overall Description
### 2.1 Product Perspective
After more that five years trading cryptocurrencies, I did face difficulties tracking positions held at various exchanges and wallets and realized nothing existed for one to track its positions. Brane is therefore a new product that will be able to talk to various crypto exchanges and wallets to centralize ease management of crypto-investments.  

### 2.2 Product Functions
- Reads cryptocurrencies balance held at exchanges and wallets  
- Provides real-time and at date portfolio balance  
- Quantitative market analysis  
- Automated trading  

### 2.3 User Classes and Characteristics
System is intended at being use by tech savyy traders and investors.  

### 2.4 Operating Environment
Brane is designed to be used on a AMD64 Debian based server.  

### 2.5 Design and Implementation Constraints
Reporting should allow investors to comply with local tax rules;  
It is intended to run 24/7 on dedicated hardware - the less resource hungry the better;  
It must connect to various exchanges and wallets;  
specific technologies, tools, and databases to be used;  
It must allow parallel operations;  
It will be developped in Julia for its numerical cimputing capabilities;  
It will used REST API to communicate with exchanges and RPC foor wallets;  
Exchanges authentication credential must be stored securely.  

### 2.6 User Documentation
Documentation will mainly be provided online/whitin software.  

### 2.7 Assumptions and Dependencies
TBD

## External Interface Requirements
### 3.1 User Interfaces
No GUI is planned at the moment, interaction with software will be done via the CLI.
### 3.2 Hardware Interfaces
- 1000BASE-T network interface for communication with wallets (within LAN)
- 1000BASE-SX uplink for communication with exchanges
### 3.3 Software Interfaces
TBD
### 3.4 Communications Interfaces
TBD

## System Features
### 4.1 Live data service
4.1.1   Description and Priority  
Priority level: High  
It allows the system to connect to cryptocurrencies exchanges and wallets to retreive user's balances and exchange rates. 
4.1.2   Stimulus/Response Sequences  
Connection is initiated on system sartup;  
Data is refreshed as often as possible.  
4.1.3   Functional Requirements  
TBD  
### 4.2 Historical data service
4.2.1   Description and Priority  
It allows the system to save data obtained from exchanges and wallets  
4.2.2   Stimulus/Response Sequences  
Live data service initiates historical data service;  
Balances and exchange rates are recorded once per minute.  
4.2.3   Functional Requirements  
TBD  
### 4.3 Other features
TBD   

## Other Nonfunctional Requirements
### 5.1 Performance Requirements
- Reporting should deliver result in less than a minute
- Quantitative analyses should deliver result in less that a second 
### 5.2 Safety Requirements
One should be able to limit value of automated trading, receive alert for trading activities and be able to get out of all position under 10 second via a panic function.  
### 5.3 Security Requirements
Authetication credential should be encrypted
### 5.4 Software Quality Attributes
System should be testable, riliable, robust and performant
### 5.5 Business Rules
User should be able to interact with system in three mode: simulation, read-only and full access.

## Other Requirements
TBD

### Appendix A: Glossary
TBD

### Appendix B: Analysis Models
TBD

### Appendix C: To Be Determined List
- 1.5 References
- 2.7 Assumptions and Dependencies
- 3.3 Software Interfaces
- 3.4 Communications Interfaces
- 4   System Features
- 5.6 Other Requirements
- Appendix
