# Anchore Training Guide Day 1

## Schedule

### Day 1

The primary objective of the first training session is educate the customer on all things Anchore. The assumption will be made that many are new to Anchore and must go through concepts, planning, and installation. At the end of Day 1 there should be a successful installation of Anchore. 

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