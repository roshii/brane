# brane
Crypto-portfolio management tool

# Software Requirements Specification
Version 0.1 in development
Prepared by roshii
2018-06-14
  
Table of Contents
=================
  * [Revision History](#revision-history)
  * [Introduction](#1-introduction)
    * 1.1 [Purpose](#11-purpose)
    * 1.2 [Document Conventions](#12-document-conventions)
    * 1.3 [Intended Audience and Reading Suggestions](#13-intended-audience-and-reading-suggestions)
    * 1.4 [Product Scope](#14-product-scope)
    * 1.5 [References](#15-references)
  * [Overall Description](#overall-description)
    * 2.1 [Product Perspective](#21-product-perspective)
    * 2.2 [Product Functions](#22-product-functions)
    * 2.3 [User Classes and Characteristics](#23-user-classes-and-characteristics)
    * 2.4 [Operating Environment](#24-operating-environment)
    * 2.5 [Design and Implementation Constraints](#25-design-and-implementation-constraints)
    * 2.6 [User Documentation](#26-user-documentation)
    * 2.7 [Assumptions and Dependencies](#27-assumptions-and-dependencies)
  * [External Interface Requirements](#external-interface-requirements)
    * 3.1 [User Interfaces](#31-user-interfaces)
    * 3.2 [Hardware Interfaces](#32-hardware-interfaces)
    * 3.3 [Software Interfaces](#33-software-interfaces)
    * 3.4 [Communications Interfaces](#34-communications-interfaces)
  * [System Features](#system-features)
    * 4.1 [System Feature 1](#41-system-feature-1)
    * 4.2 [System Feature 2 (and so on)](#42-system-feature-2-and-so-on)
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
|      |         |                     |           |
|      |         |                     |           |
|      |         |                     |           |

## 1. Introduction
### 1.1 Purpose 
This document describes requirements for a crypto-asset portfolio management tool: brane.  


### 1.2 Document Conventions
Describe any standards or typographical conventions that were followed when writing this SRS, such as fonts or highlighting that have special significance. For example, state whether priorities  for higher-level requirements are assumed to be inherited by detailed requirements, or whether every requirement statement is to have its own priority.

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
- Aggregates exchanges price data (user specific price index)
- Quantitative market analysis
- Automated trading

### 2.3 User Classes and Characteristics
Brane is intended at being use by tech savyy traders and investors.

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
Describe the connections between this product and other specific software components (name and version), including databases, operating systems, tools, libraries, and integrated commercial components. Identify the data items or messages coming into the system and going out and describe the purpose of each. Describe the services needed and the nature of communications. Refer to documents that describe detailed application programming interface protocols. Identify data that will be shared across software components. If the data sharing mechanism must be implemented in a specific way (for example, use of a global data area in a multitasking operating system), specify this as an implementation constraint.

### 3.4 Communications Interfaces
Describe the requirements associated with any communications functions required by this product, including e-mail, web browser, network server communications protocols, electronic forms, and so on. Define any pertinent message formatting. Identify any communication standards that will be used, such as FTP or HTTP. Specify any communication security or encryption issues, data transfer rates, and synchronization mechanisms.

## System Features
This template illustrates organizing the functional requirements for the product by system features, the major services provided by the product. You may prefer to organize this section by use case, mode of operation, user class, object class, functional hierarchy, or combinations of these, whatever makes the most logical sense for your product.
### 4.1 System Feature 1
Don’t really say “System Feature 1.” State the feature name in just a few words.
4.1.1   Description and Priority
 Provide a short description of the feature and indicate whether it is of High, Medium, or Low priority. You could also include specific priority component ratings, such as benefit, penalty, cost, and risk (each rated on a relative scale from a low of 1 to a high of 9).
4.1.2   Stimulus/Response Sequences
 List the sequences of user actions and system responses that stimulate the behavior defined for this feature. These will correspond to the dialog elements associated with use cases.
4.1.3   Functional Requirements
 Itemize the detailed functional requirements associated with this feature. These are the software capabilities that must be present in order for the user to carry out the services provided by the feature, or to execute the use case. Include how the product should respond to anticipated error conditions or invalid inputs. Requirements should be concise, complete, unambiguous, verifiable, and necessary. Use “TBD” as a placeholder to indicate when necessary information is not yet available.
 
 Each requirement should be uniquely identified with a sequence number or a meaningful tag of some kind.

### 4.2 System Feature 2 (and so on)

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
User should be able to contact system in three mode: simulation, read-only and full access.

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
