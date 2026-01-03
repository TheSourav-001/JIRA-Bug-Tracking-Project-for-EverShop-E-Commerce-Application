# Jira Bug Tracking – EverShop Demo Application

Project Overview:
> This repository demonstrates a complete Jira-based QA workflow applied to the EverShop demo e-commerce web application.
> Focus: defect identification, reporting, prioritization, lifecycle management, and QA–Developer collaboration.
> Purpose: Showcase practical QA skills, end-to-end defect lifecycle handling, and portfolio-ready documentation.

Application Under Test (AUT):
- Name      : EverShop Demo Web Application
- Type      : Web-based E-commerce Platform
- URL       : https://demo.evershop.io
- Modules Tested:
    > Product Listing & Category Navigation
    > Add to Cart / Cart Updates
    > Checkout Flow
    > Search & Filter Functionality
    > UI Responsiveness & Layout
    > Error Handling & Notifications

Tools & Technologies:
- Bug Tracking Tool  : Jira (Bug Tracking Template)
- Testing Method     : Manual Functional & Exploratory Testing
- Browser            : Google Chrome
- OS                 : Windows 10
- Documentation      : PDF, CSV, Screenshots
- Optional Tools     : Excel (for priority analysis), Snipping Tool (for screenshots)

Project Objectives:
- Identify functional, UI, and workflow defects
- Log defects in Jira using structured, industry-standard templates
- Prioritize defects based on severity and business impact
- Manage defects through a complete lifecycle:
    TO DO → IN PROGRESS → IN REVIEW → DONE
- Simulate QA–Developer collaboration and sprint-based workflow
- Generate workflow proof and reporting artifacts suitable for portfolio presentation

Scope of Testing:
+ In Scope:
    - Product Listing, Categories & Navigation
    - Add to Cart / Cart Updates
    - Checkout Process Validation
    - Search & Filter Functionality
    - UI Responsiveness & Layout across screen sizes
    - Validation of error messages & notifications
+ Out of Scope:
    - Payment Gateway & Transactions
    - Backend/Database Integration
    - Performance, Load, Security & Stress Testing

Defect Management Approach:
- All defects logged as Jira Bug issues
- Template Fields Used:
    Summary | Environment | Steps to Reproduce | Expected Result | Actual Result | Severity | Priority
- Workflow: 
    ```
    TO DO → IN PROGRESS → IN REVIEW → DONE
    ```
- Purpose: Reflects a **real-world Agile defect management lifecycle**

Bug Prioritization:
- High    : Critical business-impacting issues (blocking checkout, add to cart failures)
- Medium  : Functional issues with available workarounds
- Low     : Minor UI inconsistencies, cosmetic issues

Workflow Simulation:

[Step 1] TO DO - Defect Logging
--------------------------------
- QA identifies defect during exploratory testing
- Example Defect:
    > Summary      : "Add to Cart button not responding for certain products"
    > Environment  : Chrome 117, Windows 10
    > Steps        : 
        1. Open product page
        2. Click Add to Cart
        3. Observe behavior
    > Expected     : Product should be added to cart
    > Actual       : Button appears unresponsive
    > Severity     : High
    > Priority     : High
- Status set to TO DO
- Assignee    : Unassigned
- Jira Comment: "Defect logged for initial review"

[Step 2] IN PROGRESS - Developer Assignment
-------------------------------------------
- High priority defects assigned to developer
- Status changed to IN PROGRESS
- Jira Comment:
    > "Developer has started investigating the issue. Root cause analysis in progress."
- Medium priority defects remain in TO DO (backlog)
- Low priority defects deferred for future sprints

[Step 3] IN REVIEW - QA Verification
------------------------------------
- Developer applies fix for high priority defect
- Status changed to IN REVIEW
- QA verifies functionality
- Example Jira Comment:
    > "Fix completed by developer. Ready for QA review."
- Medium priority defects moved to IN PROGRESS as sprint allows
- Low priority defects remain in TO DO

[Step 4] DONE - Fix Completion & Closure
----------------------------------------
- QA validates fix
- Status updated to DONE
- Example Jira Comment:
    > "Fix validated by QA. Issue behavior matches expected outcome."
- Medium priority defects remain IN REVIEW
- Low priority issues deferred

Repository Structure:
------------------------------------
```
Jira-Bug-Tracking/
├── Bug-List-Export/
│   └── EverShop_Jira_Bug_List.csv      # CSV export of all defects with priorities
├── Sample-Bugs/
│   ├── ESBUG-3_Add_To_Cart_Issue.pdf
│   ├── ESBUG-6_Checkout_Issue.pdf
│   └── ESBUG-8_UI_Layout_Issue.pdf
├── Reports/
│   ├── Bug_Status_Distribution.png      # High/Medium/Low defect chart
│   └── Priority_Analysis.png            # Pie chart of defects by severity
└── Workflow-Proof/
    ├── 01_All_Bugs_Logged_Status_TODO.png
    ├── 02_High_Priority_Bugs_In_Progress.png
    ├── 03_Bugs_In_Review_And_In_Progress.png
    └── 04_High_Priority_Bugs_Completed_Medium_In_Review.png
```

Key Learnings:
- Hands-on Jira defect tracking experience
- Complete defect lifecycle understanding
- Priority-based QA decision-making and backlog management
- Realistic QA–Developer workflow simulation
- Professional reporting & documentation practices

Author: Sourav Dipto Apu
--------------
Focus: Manual Testing, Jira Bug Tracking, Defect Lifecycle Management, QA Documentation

Disclaimer:
> This project was created for QA practice and portfolio demonstration purposes.
> Only public demo applications were used. No production systems or real user data involved.

ASCII Workflow Overview:
------------------------
```
TO DO         : Initial defect logging
   │
   ▼
IN PROGRESS   : Developer assigned, fix in progress
   │
   ▼
IN REVIEW     : QA validation of fixes
   │
   ▼
DONE          : Fix completed and verified
```
