# Anchore Training Guide Day 2

## Schedule

### Day 2

The primary objective of the second training day is educate the customer on usage of Anchore. 

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
