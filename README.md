# FY22-Q2-AI-Hackathon-Anomaly-Detection

### Proposed Topic: Early detection of documents having increased chances of publishing error.

**ABCD (Application Bundle for Creating Documents)** is a mission critical client application accessed by large number of users from Legal and Pricing team. 
One of the primary app function is to publish new custom document packages from multiple document templates and rate tables. Publishing this document packages in a timely fashion is critical for client business. All documents are expected to be Auto Published. Any major delays will invite penalties and sanctions from government entities.
A document is considered Auto Published if it gets successfully published the same day or next day. If the document do not get Auto Published, it will require manual intervention. The investigation will be done by a technical team and the document republished using an alternate manual process at the earliest. 

### Current Approach
* Client has tasked Accenture to help increase Auto Publish % and thus reduce the risk of inviting penalties. 
* The team is expected to identify and resolve issues within 24 hours. 
* Have implemented Database Alerting. Technical team will receive alerts once the issue happens (Auto Publish Indicator = N). 

### Problem Statements
* Current approach of detecting issue and republishing manually is reactive in nature. 
* The team comes to know about the issue only after it happens. A delay of 24 to 47 hours before the issue is identified.
* Bare minimal time for correction and republishing. Tight SLA - team under pressure to fix the issue within 24 hours. 
* Higher risk of missing SLAs - for both Accenture Technical teams and Client.
* 24x7 support from technical teams required, thus increasing cost.

### Proposed Solution
* Attempt to create a ML based Anomaly detection model which has the ability to predict with certain confidence the document packages that has increased chances of failing Auto Publishing.

### Benefits
* Technical team will be alerted on document packages having increased chances of failing Auto Publish, at the time of Approval.
* Technical team can monitor risky packages closely and line up resources accordingly.
* Can educate client if patterns of incorrect usage identified.
* Staffing support team as needed based on census and recommendations received. Reduced cost for Accenture.
* Reduced risk of penalties. Increased Customer Satisfaction.

#### Notes:
🧑 Auto Publish indicator is set as Y when the difference of Package Published Date and Package Approved Date equals 0 or 1. It will be N otherwise.

🧑 A blank value in Package Published Date will indicate the document package is not yet published. It can be treated as Not Auto Published.


