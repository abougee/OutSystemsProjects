Welcome to the consulting revenue insights portal. 

This application supports documentation of clients, their engagement project details, the project's relevant engagement teams,
project billing milestones and project revenue recognitions.

The following static entities in this project are setup as follows:
1. Client Status: Active, Inactive.
2. Currency Entity: USD, EUR.
3. Engagement Type: Advisory, Implementation.
4. Industry: Financial Services, Healthcare.
5. Region: North America, Europe.
6. Consultant Seniority Level: Analyst, Partner.
7. BillingMilestone/Engagement Status: Pending, In Progress, Completed, Cancelled.

The entities in this project are setup as follows:
1. Client:
   a. Name.
   b. IndustryId.
   c. RegionId.
   d. AccountOwnerId (UserId).
   e. Client StatusId   

2. Consultant:
   a. Role
   b. Office.
   c. SeniorityLevelId.
   d. DailyRate.
   e. ActivityStatus

3. Engagement:
   a. ClientId.
   b. Name.
   c. StartDate.
   d. EndDate.
   e. EngagementTypeId.
   f. Engagement StatusId.
   g. Contract Value.
   h. Currency Id.
   i. Delivery Probability.
   j. Expected Revenue.

4. EngagementTeam:
   a. EngagementId.
   b. ConsultantId.
   c. RoleOnEngagement.
   d. Start Date.
   e. End Date.

5. BillingMilestone:
   a. EngagementId.
   b. Milestone Name.
   c. Due Date.
   d. Amount.
   e. Billing Milestone StatusId.

6. Revenue Recognition:
   a. EngagementId.
   b. Announced Month.
   c. Recognized amount.
   d. Forecast amount.
   e. Confidence Level.

The portal application allows login with the following sample profiles:
1. Jesse Hernandez. Role: Administrator.
2. Matthew Shelton. Role: Account Manager.
3. Jerry Harris. Role: Consultant
4. Default community provider (For developers)

This portal application supports the following pages with the following features:
1. Dashboard
   a. Contains card for total contract values.
   b. Contains card for total Outstanding (not completed) Billing amounts.
   c. Contains card for total recognized revenue amounts.
   d. Contains card for total forecasted revenue amounts.
   e. Contains average margin or engagement probabilities.
   f. Contains line chart for revenues by month.
   g. Contains donut chart for revenues by industry.
   h. Contains bar chart for pipelined engagements by status.
   i. Overdue Billing milestones list containing the top 5 pending or InProgress Biling milestones.
   j. Clients list containing the top 5 clients by contract value.


2. Clients List where you can filter by name search, Region, industry and client activity status.

3. Engagements List where you can filter by name search, Client name, engagement type, engagement status and utilized currency.

4. Engagement details within Engagement list item entailing an overview, relevant Engagement teams, relevant billing milestones and 
relevant revenue recognitions.

5. Consultants List where you can filter by name search and Seniority Level. 

6. Billing Milestones where you can filter by name search, Engagement title and Billing milestone status.

7. Revenue Recognitions where you can filter by Engagement name search and Engagement title.

8. Import and export page (underneath user profile logo) 
for Clients, Engagements, Engagement Teams, Consultants, Billing milestones andd revenue recognitions.


The following roles and their responsibilities are as follows:

1. Administrators:
   a. Can view dashboard.
   b. Can view, create and edit clients.
   c. Can view, create and edit engagements.
   d. Can view, create and edit engagement teams.
   e. Can view, create and edit consultants.
   f. Can view, create and edit billing milestones.
   g. Can view, create and edit revenue recognitions.
   h. Can view import and export sheet page to download and upload excel sheets.

2. Account Managers:
   a. Can view dashboard.
   b. Can view clients, but cannot create or edit them.
   c. Can view engagements, but cannot create or edit them.
   d. Can view, create and edit engagement teams.
   e. Can view, create and edit consultants.
   f. Can view, create and edit billing milestones.
   g. Can view, create and edit revenue recognitions.

3. Consultants:
   a. Can view dashboard.
   b. Can view billing milestones, but cannot create or edit them.
   c. Can view revenue recognitions, but cannot create or edit them.




