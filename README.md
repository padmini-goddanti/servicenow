**Automated Network Request Management in ServiceNow**

**Project Overview**

Automated Network Request Management is a ServiceNow-based project designed to manage network-related service requests efficiently through a structured and automated process.

**Objective**

The business objective for Automated Network Request Management in ServiceNow typically aligns with improving operational efficiency, reducing manual effort, and enhancing user satisfaction in managing network-related services
To streamline and automate the end-to-end lifecycle of network-related service requests using ServiceNow, thereby:
· Reducing manual effort and human error
· Accelerating request fulfilment times
· Enforcing standardized workflows and approval processes
· Improving visibility and tracking through a centralized platform
· Enhancing end-user experience with faster, more reliable service delivery
· Ensuring compliance with IT and security policies


**Functinal scope**
Covers catalog creation, form design, approval routing, flow designer automation, and email notifications.

**Execution Roadmap**
Roadmap divided into milestones:
-catalog creation, 
-form setup, 
-approval integration, 
-testing
-deployment.

**Catalog creation**
Objective: Establish a structured, user-friendly service catalog for network requests.
·        Identify network request types
·        Define request catalogs and categories.
·        Create service catalog items with clear titles and descriptions.
·        Collaborate with network and IT teams for content accuracy.
·        Ensure catalog taxonomy aligns with ITSM structure.
**Form setup**
Objective: Design dynamic, intuitive forms that capture all required request data.
·        Build catalog item forms using variables.
·        Add dynamic behaviours (show/hide fields based on selection).
·        Include mandatory fields to reduce incomplete submissions.
·        Align form inputs with downstream automation and workflows.
**Approval integration**
Objective: Automate and enforce approval workflows for compliance and control.
·        Identify required approval chains (e.g., manager, network security).
·        Configure approval steps using Flow Designer or Workflow Editor.
·        Ensure audit logging and email notifications are enabled.
**Testing**
Objective: Validate end-to-end request lifecycle and automation.
·        Perform unit testing on each catalog item.
·        Conduct end-to-end request simulation with multiple scenarios.
·        Validate approvals, task creation, notifications, and data accuracy.
·        Involve stakeholders in UAT (User Acceptance Testing).
·        Log defects and iterate improvements.
**Deploymen**
Objective: Launch automated request management in the production environment.
·        Finalize deployment checklist.
·        Migrate workflows and catalog items from development to production.
·        Monitor system behaviour and performance post-launch.
·        Provide training to end users and fulfilment teams.
·        Setup support process for post-deployment issues.

PHASE 2:BACKEND DEVELOPMENT AND CONFIGURATIONS
-----Develop the core logic, configure system settings, and set up backend integrations and automations.----
**Data Architecture**
--The Automated Network Request Management solution in ServiceNow is built using a structured data model that combines standard platform tables with a custom network request table to ensure clarity, scalability, and control. Network requests are captured through catalog-driven records and stored with well-defined fields such as request type, access level, business justification, and related network configuration items. Forms are designed to dynamically display only relevant information using UI logic, while mandatory fields enforce data accuracy and compliance. List views provide operational visibility for approvers and network teams, enabling efficient tracking of requests, tasks, and statuses. This architecture ensures secure access, seamless automation, and reliable reporting across the entire request lifecycle.

PHASE 3:UI/UX DEVELOPMENT & CUSTOMIZATION
-----Design user-friendly interfaces and customize layouts to enhance usability and brand consistency.
1.Interface Design:
       Designing and customizing ServiceNow interfaces—like forms, lists, and Service Portals—to ensure a user-friendly experience that aligns with business needs, using tools such as UI Policies, UI Actions, and the ServiceNow UI Builder.
2.Navigation Flow
3.UI Policy

PHASE 4:DATA MIGRATION ,TESTING AND SECURITY
-----Migrate data securely, perform rigorous testing, and ensure system access and data protection mechanisms are in place.
1.Automation:
     Implemented Flow Designer logic: Get Catalog Variables, Create Record, Ask for Approval, Send Email, Update Record.
     Triggered on catalog item submission; supports dynamic automation.
2.Access control
3.QA Testing
4.Data integrity:
      Field Validation and Automation
            ·        Mandatory Fields: Enforced on client and server side to prevent incomplete submissions.
            ·        Auto-Populate Logic: Set up default values (e.g., current user, location) using catalog client scripts and UI policies.
            ·        Approval State Validation: Ensured that a request cannot progress unless the required approval is completed using flow conditions and approval state checks in the workflow.
       

**Project Workflow**

1. The user selects the required network service.
2. The user provides the required information through catalog variables.
3. The request is submitted through ServiceNow.
4. The request is processed according to the configured workflow.
5. Approval is obtained when required.
6. The request can be tracked and managed through ServiceNow.

**Innovation**
-----· Implemented end-to-end automation using:
·        Flow Designer (no custom script includes or business rules)
·        Dynamic approvals and task creation
·        Client scripts and UI policies kept to minimal, essential use
· Ensured maintainability and ease of handoff to admins or future developers.

**Functional overview**
· Variables:
·        Request type, justification, Portal details, urgency
· Approval Use Cases:
·        Manager approval for standard requests
·        Network security approval for high-sensitivity requests
·        Group approval for department-specific tasks

**SCalability & future plan**
--Future enhancements considered:
·   Auto-provisioning via integrations with network tools (e.g., Cisco DNA Centre, Ansible)
·   Orchestration flows using ServiceNow Integration Hub
·   Reporting dashboards for request volume, fulfilments, and etc.
·   Expansion to other IT services (e.g., device provisioning, access requests)

**Project conclusion**
The Network Request Management system in ServiceNow automates request intake, routing, and fulfillment. Through dynamic forms, role-based approvals, and email notifications, it ensures transparency and efficiency. Optional automation integration further reduces manual workload and risk, enabling faster and more reliable network operations.
