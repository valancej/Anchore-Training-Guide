# Day 2 Detailed Schedule

The primary objective of the second training day is educate the customer on proper usage of Anchore. At the end of day 2, the customer should have a working installation of Anchore configured correctly, and know how to properly operate it. 

**Note:** Topics with a '*' may not be necessary depending on use case (OSS or Enterprise).

- **Introduction**
    - Answer any outstanding question from previous training session.
    - Introduce topics that will be covered during training session today.
- **Configuring Anchore (No integrations)**
    - [Registry Configuration](https://anchore.freshdesk.com/support/solutions/articles/36000003888-configuring-access-to-registries)
    - [Registry Configuration through UI](https://anchore.freshdesk.com/support/solutions/articles/36000100422-ui-configuring-private-registries)*
    - [Adding images](https://anchore.freshdesk.com/support/solutions/articles/36000003482-adding-images)
    - [Adding images through UI](https://anchore.freshdesk.com/support/solutions/articles/36000100263-ui-analyzing-images)*
    - [Repository scanning](https://anchore.freshdesk.com/support/solutions/articles/36000023659-scanning-repositories)
- **Configuring Anchore (Integrations)**
    - Co-build image pipeline with Anchore.
    - [Jenkins Plugin Site](https://plugins.jenkins.io/anchore-container-scanner)
    - [Gitab Integration Documentation](https://anchore.freshdesk.com/support/solutions/articles/36000058199-gitlab-integration)
    - Other CI documentation to follow.
    - [Working with subscriptions and webhooks](https://anchore.freshdesk.com/support/solutions/articles/36000003890-working-with-subscriptions)
- **Policy Deep Dive**
    - [Policies Overview](https://anchore.freshdesk.com/support/solutions/articles/36000074706-policies)
    - [Policy Bundles](https://anchore.freshdesk.com/support/solutions/articles/36000074705-policy-bundles-and-evaluation)
    - [Complete List of Policy Checks](https://anchore.freshdesk.com/support/solutions/articles/36000073896-anchore-policy-checks)
    - [Policy Mappings](https://anchore.freshdesk.com/support/solutions/articles/36000054291-policy-mappings)
    - [Working with Policies](https://anchore.freshdesk.com/support/solutions/articles/36000003885-working-with-policies)
    - [Managing Policy Bundles UI](https://anchore.freshdesk.com/support/solutions/articles/36000054295-managing-policy-bundles)*
    - [Trusted and Blacklisted Images UI](https://anchore.freshdesk.com/support/solutions/articles/36000054292-trusted-and-blacklisted-images)*
    - [Whitelists UI](https://anchore.freshdesk.com/support/solutions/articles/36000054290-whitelists)*
- **Policy Creation & Integration**
    - Co-build policies based on organizational requirements and infomation obtained above.
    - [Evaluating Policies](https://anchore.freshdesk.com/support/solutions/articles/36000003457-evaluating-images-against-policies)*
    - [Testing Policies UI](https://anchore.freshdesk.com/support/solutions/articles/36000054293-testing-policies)*
    - Ensure that all policies are created and integrated successfully as needed. 
- **Anchore Configuration & wrap-up**
    - [Accounts and Users](https://anchore.freshdesk.com/support/solutions/articles/36000098273-accounts-and-users-engine-v0-3-0-)
    - [Managing Accounts and Users](https://anchore.freshdesk.com/support/solutions/articles/36000098274-managing-accounts-and-users)
    - [RBAC Concepts](https://anchore.freshdesk.com/support/solutions/articles/36000098090-role-based-access-control)*
    - [RBAC Configuration UI](https://anchore.freshdesk.com/support/solutions/articles/36000098542-ui-managing-users-accounts-and-roles-with-rbac)*
    - [Event Log](https://anchore.freshdesk.com/support/solutions/articles/36000069073-event-log)
    - Troubleshooting
        - Walkthrough accessing logs in specific containers.
    - Answer any outstanding technical questions and wrap up.
