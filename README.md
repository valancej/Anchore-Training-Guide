# Anchore Training Guide

## Table of Contents

<!--ts-->
  * [Introduction](#Introduction)
  * [Training Schedule Overview](#Training-Schedule-Overview)
    * [Day 1](#Day-1)
    * [Day 2](#Day-2)
  * [Planning and Installation Guides](Planning-and-Installation-Guides)

<!--te-->

## Introduction

The intent of this document is to serve as a structured reference for Anchore New Customer Training. This document will walkthrough an Anchore Overview, Concepts, and Planning. Following a solid planning of Anchore, the appropriate install guide will be selected for walkthrough. Once the installation has been completed successfully, Anchore customers will receive a walkthrough of the operational functions of Anchore.

## Training Schedule Overview

This customer training is designed to be spread over 1-2 working days, with the majority of the first day being deticated to overview, planning and install. The second day (if necessary) will be reserved for Anchore training of users. 

### Day 1

The primary objective of the first training session is educate the customer on all things Anchore. The assumption will be made that many are new to Anchore and must go through concepts, planning, and installation. At the end of Day 1 there should be a successful installation of Anchore. 

[View Day 1 Directory](https://github.com/valancej/Anchore-Training-Guide/tree/master/day_1)

- **10:00 - 11:00 AM (Hour 1) - Introductions**
    - Anchore and customer introductions. Develop a clear understanding of roles (who will be the Anchore power users).
    - Overview of Anchore, architecture (services), the approach we take to image scanning (image analysis lifecycle), where we fit into the container lifecycle, common customer use cases, general Anchore concepts. 
- **11:00 - 12:00 PM (Hour 2) - Anchore Planning Guide Walkthrough**
    - Complete walkthrough and throughout understanding of what is takes to get Anchore up and running. This will be dependent on a number of factors outlined in the formal guide. Capacity planning will come at the end of this, however no deticated infrastructure will be provisioned at this time.
    - Main goal of this section is to gain a solid understanding of where Anchore will live, how Anchore will be deployed, and what are the primary objectives the customer will be leveraging Anchore for?
    - What are the points of integration? CI/CD, watching repositories in registries, or both? Will there be alerting or ticketing set up? Is the Enterprise UI going to be leveraged at all or is client interaction done via the API/CLI?
    - What are the container registries that Anchore will need access to? Are this public or private?
    - Seeing the planning guide for networking/capacity etc..  
- **12:00 - 1:00 PM - Break**
- **1:00 - 2:00 (Hour 3) - Installation Planning**
    - Folowing the Planning Guide Walkthrough all of the above questions should be answered along with questions that come up organically by following the guide. 
    - Resources can be provisioned at this time based on the usage ans answers from the previous steps. This includes VMs (appropriate capacity), network access for feeds. 
    - What is the final approach the customer will be taking? If through CI what does the architecture look like (surrounding tools? staging and production registries?)
    - If webhooks are being used, are there mechanisms in place for consuming them? 
- **2:00 - 3:00 PM (Hour 4) - Installation**
    - Once all planning has been completed, Anchore customer can select which install guide to follow and begin to install the software requirements on provisioned infrastructure, and install Anchore.
    - Walkthrough any necessary, Anchore-specific configurations at this time. 
- **3:00 - 3:30 PM (30 min 1) - Break**
- **3:30 - 4:00 PM (30 min 2) - Wrap up**
    - Address any outstanding planning, installation, and configuration questions that may have come up throughout the day.
    - Overview of what is to come during the next training session.

### Day 2

The primary objective of the second training day is educate the customer on proper usage of Anchore. At the end of day 2, the customer should have a working installation of Anchore configured correctly, and know how to properly operate it. 

[View Day 2 Directory](https://github.com/valancej/Anchore-Training-Guide/tree/master/day_2)

- **10:00 - 10:30 AM (30 min 1) - Introductions**
    - Introduce topics for the day and address anything outstanding from the previous training session.
- **10:30 - 11:30 AM (Hour 1) - Configuring Anchore (No integrations)**
    - Walkthrough of configuring necessary container registries and scanning images from end to end. This wil be dependent on the information gathered in the planning session the previous training day. 
    - This will include common ways of interacting with Anchore to scan images. Examples will include CLI and API interaction to add registries and images. UI if necessary. 
    - End goal of this hour is to make sure all images the user would like to scan with Anchore are able to be scanned. 
    - No integrations at this time.
- **11:30 - 12:30 PM (Hour 2) - Configuring Anchore (Integrations)**
    - Walkthrough on configuring Anchore for the use case information captured from the previous training session. 
    - Co-build the CI pipeline to ensure built images are able to be scanned with Anchore successfully. 
    - Co-build the repositories/tags that the customer would like to be put in 'watch' mode. 
    - Configure any alerting webhooks if necessary.
- **12:30 PM - 1:30 PM - Break**
- **1:30 PM - 2:30 PM (Hour 3) - Policy Deep Dive**
    - Overview of Anchore policies, how they work (some of this will be covered in the previous training session).
    - Go through each policy gate and trigger with examples.
    - What are the policies the customer would like to be built? 
    - How will these policies be enforced? If at all.
- **2:30 - 3:30 PM (Hour 4) - Policy Creation & Integration**
    -  Co-build the policies with the customer (UI, API, CLI).
    - Integrate the policies into CI pipeline build in previous step.
    - Integrate the policies via alerting and ticketing if needed. 
- **3:30 - 4:30 PM (Hour 5) - Anchore Configuration & wrap-up**
    - Enterprise customers will get a UI walkthrough at this time. 
    - Troubleshooting (logs)
    - Post-installation configuration tasks (if necessary).
    - Address any outstanding technical or non-technical questions from the past two training sessions.
    - Wrap up.

## Planning and Installation Guides

- [Anchore Planning Guide](https://github.com/valancej/Anchore-Documentation/blob/master/docs/planning/planning-guide.md)
- [Anchore Installation Documentation](https://github.com/valancej/Anchore-Documentation)