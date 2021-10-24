# ML_Building
Predict the Building Permission Category 

## Problem Description
Nowadays, we are living in a concrete world, tall and small buildings here and there, everywhere. But some of them are constructed without any 
proper permission or documents, while some of the genuine buildings get stuck due to permission delay issues, etc. Here's a dataset of building 
permissions, which consists application date, expiration date, permission granted or not, location, description etc. Based on all these features 
given you have to predict which category does the building permission fall into.

There are typically 5 categories: 
1. Single Family / Duplex
2. Commercial 
3. Multifamily 
4. Institutional
5. Industrial 

You have to predict the column "Category". 

## Data Description 
The columns in the data are described as follows: 

| SI. No. | Column Label | Column Description |
| ------------- | ------------- | ------------- |
| 1 | Application/Permit Number  | The tracking number used to refer to this application or permit record in various Seattle DCI tracking systems. |
| 2 | Permit Type  | Type of activity covered by the permit. |
| 3 | Address | Street address of the work site. |
| 4 | Description | Brief description of the work that will be done under this permit. This is subject to change prior to issuance of the permit, but generally more stable if an issue date exists. Very long descriptions have been truncated.|
| 5 | Action Type | Subclassification for type of work being proposed. Valid choices will vary depending on the permit type. |
| 6 | Work Type | An indicator of the complexity of the project proposed. Easier projects can be issued without plan review: more complex projects generally require plan submittal and review. |
| 7 | Applicant Name | The name of the person or company listed on the application as the "primary applicant". This may be the property owner, contractor, design professional, or other type of agent. |
| 8 | Application Date | The date the application was accepted as a complete submittal. If no Application Date exists this generally means the application is in a very early stage. |
| 9 | Issue Date | The date the application was issued as a valid permit. If an Application Date exists but no Issue Date exists, this generally means the application is still under review. |
| 10 | Final Date | The date the permit had all its inspections completed. If an Issue Date exists but no Final Date exists, this generally means the permit is still under inspection. |
| 11 | Expiration Date | The date the application is due to expire. Generally, this is the date by which work is supposed to be completed (baring renewals or further extensions). If no Expiration Date exists, this generally means the application is has not been issued yet. |
| 12 | Status | The current status in the application/review/inspection lifecycle. Indicates the last process step that was fully completed. |
| 13 | Contractor | Contractor(s) who are associated with this permit. |
| 14 | Permit and Complaint Status URL | Link to view full details and current status information about this permit at Seattle DCI's website. |
| 15 | Master Use Permit | A Master Use/Land Use Permit is required before some building permits to make decisions about site-specific factors of the project, such as environmental impacts or neighborhood design considerations. |
| 16 | Latitude | Latitude of the worksite where permit activity occurs. May be missing for a small number of permits considered "Unaddressable" |
| 17 | Longitude | Longitude of the worksite where permit activity occurs. May be missing for a small number of permits considered "Unaddressable" |
| 18 | Location | Mapping coordinates for the permit address. |
| 19 | Category | The broad category of use or occupancy for the building where work is proposed. Valid choices are Commercial, Industrial, Institutional, Multifamily, and Single Family/Duplex. Mixed use structures are generally represented as Commercial. |


## Evaluation Metrics 
The submissions will be evaluated based on Fl Score with 'weighted' average.
