# COMP5047 Task 3a: Specification and Modelling Software Functional Requirements, Use Case Model
**Subsystem:** USU Operation System  

---
Below is an outline of the 7 use cases (UC) for USU operation system. 

<details>
<summary>UC-01: Approving USU Membership</summary>

## UC-01: Approve USU Membership
**Primary Actor:** USU Officer  
**Secondary Actor:** Union Officer  
**System:** USU OS  

USU Officer reviews and approves a membership application submitted by a university-specific student union, activating the union account and enabling access for its officers and student members.

### Entry Conditions
- Union membership application submitted
- USU Officer logged in with approval permissions

### Exit Conditions (Success)
- Union account activated
- Union Officers’ system accounts created
- Students from the university can register
- Union can participate in USU events
- Notification sent to Union Officer

### Main Flow
| Union Officer | USU Officer | System |
|---|---|---|
| Submits membership request | — | Records and validates request |
| — | Opens pending membership list | Displays list |
| — | Selects application | Shows application data |
| — | Reviews request | Waits for decision |
| — | Approves request | Activates account, creates access, notifies UO |

### Exceptional Flows
- Missing/incomplete data → request returned for correction
- Invalid data → request rejected, notification sent
- System error → error logged, manual intervention required

</details>



<details>
<summary>UC-02: Approve Updates to USU Membership</summary>

## UC-02: Approve Update to Union Data
**Primary Actor:** USU Officer  
**Secondary Actor:** Union Officer  
**System:** USU OS  

Union Officer submits request to update registration information, which USU Officer reviews and approves.

### Entry Conditions
- Union has active membership
- Data update request submitted

### Exit Conditions
- Union data updated
- Audit log recorded
- Notification sent to Union Officer

### Main Flow
| Union Officer | USU Officer | System |
|---|---|---|
| Submits update request | — | Validates and stores request |
| — | Opens pending update list | Displays pending requests |
| — | Selects request | Shows current vs new data |
| — | Reviews request | Waits for decision |
| — | Approves update | Applies changes, logs update, notifies UO |

### Exceptional Flows
- Invalid or missing information → request returned
- Unauthorized change → request rejected
- System error → logged, admin required

</details>

<details>
<summary>UC-03: Approve Termination of Membership</summary>

## UC-03: Approve Termination of Membership
**Primary Actor:** USU Officer  
**Secondary Actor:** Union Officer  
**System:** USU OS  

USU Officer reviews and approves a union’s request to terminate membership.

### Entry Conditions
- Termination request submitted
- USU Officer logged in

### Exit Conditions
- Union account marked inactive
- User access disabled
- Data scheduled for deletion after 1 month
- Union notified

### Main Flow
| Union Officer | USU Officer | System |
|---|---|---|
| Submits termination request | — | Records request |
| — | Reviews request | Validates union & pending events |
| — | Approves termination | Deactivates account |
| — | — | Schedules data deletion, sends notification |

### Exceptional Flows
- Pending events/members → request rejected
- System failure → error logged, admin action needed
</details>

<details>
<summary>UC-04: Create New Event</summary>

## UC-04: Create New Event
**Primary Actor:** USU Officer  
**Secondary Actor:** Union Officer  
**System:** USU OS  

USU Officer creates and publishes a new event, enabling student and union interaction.

### Entry Conditions
- USU Officer logged in with event-creation permissions

### Exit Conditions
- Event created and published
- Notifications sent to Union Officers and students
- Event opened for subscription and endorsement

### Main Flow
| USU Officer | System |
|---|---|
| Opens create event form | Displays form |
| Enters event details | Validates inputs |
| Submits event | Saves event, publishes it |
| — | Sends notifications, enables participation tools |
| Receives confirmation | Shows success message |

### Exceptional Flows
- Missing/invalid data → correction requested
- Event conflict detected → warning shown, user decides
- Save/publish failure → logged, retry required


</details>

<details>
<summary>UC-05:  Update Event / Publish Announcements</summary>

## UC-05: Update Event / Publish Announcements
**Primary Actor:** USU Officer  
**Secondary Actors:** Student, Union Officer  
**System:** USU OS  

USU Officer posts event announcements and progress updates.

### Entry Conditions
- Event already created

### Exit Conditions
- Update visible
- Notifications delivered

### Main Flow
| USU Officer | System |
|---|---|
| Selects event | Displays event info |
| Enters announcement/update | Validates content |
| Submits update | Publishes update, notifies users |

### Exceptional Flows
- Invalid content → correction requested
- Notification failure → logged and retried

</details>

<details>
<summary>UC-06: Student Participation in Events</summary>

## UC-06: Student Participation in Events
**Primary Actor:** Student  
**Secondary Actor:** Union Officer  
**System:** USU OS  

Students subscribe to event information and/or register to participate.

### Entry Conditions
- Student registered and logged in
- Event is open for registration

### Exit Conditions
- Student subscription/registration recorded
- Notifications sent

### Main Flow
| Student | System |
|---|---|
| Searches/chooses event | Shows available events |
| Selects actions (subscribe/register) | Checks eligibility |
| Confirms | Records participation and sends confirmation |

### Extensions (from diagram)
- Join Waiting List
- Cancel Participation
- Accept Registration Closed
- Accept Ineligible to Register

### Exceptional Flows
- Event full → waiting list option
- Registration closed → blocked, message shown
- Invalid student → rejected
</details>

<details>
<summary>UC-07:  Union Endorsement of Events</summary>

## UC-07: Union Endorsement of Events
**Primary Actor:** Union Officer  
**Secondary Actor:** USU Officer  
**System:** USU OS  

Union Officer endorses events on behalf of their university.

### Entry Conditions
- Union Officer logged in
- Event open for endorsement

### Exit Conditions
- Endorsement recorded
- Notifications sent

### Main Flow
| Union Officer | System |
|---|---|
| Views event list | Shows endorsable events |
| Selects event | Validates eligibility |
| Endorses event | Records endorsement, notifies USU Officer |
| Confirms action | Shows success state |

### Extensions
- Cancel Endorsement
- Accept Event Ineligible to Endorse
- Accept Event Unavailable to Endorse

### Exceptional Flows
- Endorsement window closed → error shown
- Unauthorized → access denied
- System error → logged, retry later

</details>


<img width="2180" height="981" alt="USUSubsystem" src="https://github.com/user-attachments/assets/ff0dd79a-4b83-490b-9d07-c59216d59c0d" />
