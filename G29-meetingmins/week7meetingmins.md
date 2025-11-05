# COMP5047 Applied Software Engineering  
## Group G29 – Week 7 Meeting Agenda & Minutes  

**Date:** 04/11/25  
**Time:** 14:00–15:45  
**Location:** Google Meet  

**Attendees:**  
- David Gaman (19238600)  
- Aziz Hussein Boakye (19067039)  
- Areebah Khan (19343387)  
- Daniil Tkachenko (19323083)  

All Present  

---

## Agenda

1. Final review of Task 3 (Use Case & Activity diagrams).  
2. Start Task 4a planning for each subsystem (microservices-based component architecture).  
3. Clarify which microservices each subsystem provides and which they request from others.  
4. Cross-check consistency across subsystems (boundaries, interfaces, naming).  
5. Review GitHub commits and folder structure for Task 4.  
6. Assign actions so everyone has an initial draft of 4a before Week 8.  

---

<details>
<summary>Progress Since Last Meeting</summary>

- All members are comfortable with Papyrus for UC and Activity diagrams; shared more layout/formatting tips.
- Task 3 status:  
  - David: Task 3 complete.  
  - Daniil: Task 3 complete (updated per lecturer feedback).  
  - Aziz: UC complete, Activity nearing completion.  
  - Areebah: Task 3 complete and committed.  
- Everyone reviewed Week 6 lecture notes to prepare for Task 4.
- Regular contact maintained via WhatsApp.

</details>

---

<details>
<summary>Key Decisions</summary>

- Begin Task 4a this week as planned in Week 6.
- Each member to draft a microservice list and component diagram for their subsystem.
- Use consistent naming structure (`*Service`, `*Gateway`, `*Adapter`, etc.).
- Clearly label provided vs required interfaces in diagrams.
- Share early drafts in group chat for feedback before final commits.
- Avoid losing commit history by using GitHub rename/move, not drag–reupload.

</details>

---

<details>
<summary>Discussion</summary>

### Task 3 Wrap-Up
- Tidied UC & Activity diagrams (alignment, labels, straight connections).
- Confirmed swimlanes + object flows included to meet marking criteria.
- Ensured diagrams align with functional requirements in the case study.

### Task 4a – Subsystem Architecture (Microservices)
- Discussed component diagram structure:
  - Subsystem boundary box
  - Internal microservices
  - Provided + required interfaces
- Agreed to describe each microservice in one line to maintain consistency.
- Agreed to show interface operations as names only for now (parameters later).
- Confirm consistent naming across systems for shared entities (UnionId, EventId, etc.).

### Early Microservice Ideas (to refine individually)
- **USU Operation System (Areebah)**  
  `UnionMembershipService`, `UnionDataApprovalService`, `EventManagementService`, `USUNotificationAdapter`

- **Student Union Management System (Aziz)**  
  `UnionRosterService`, `UnionProfileService`, `UnionEventEndorsementService`, `SUNotificationAdapter`

- **USU Student App (David)**  
  `StudentProfileService`, `EventSubscriptionService`, `TicketingClient`, `StudentNotificationGateway`

- **Society Leader App (Daniil)**  
  `SocietyManagementService`, `SocietyEventService`, `OfficerAccessGateway`

### GitHub
- Work stored in `/uml/task4/` and `/docs/task4/`.
- Commit messages must reference task + subsystem.
- Keep work inside repository (no external editing).

### Preparation for Next Week
- Each member to bring a draft component diagram + service list.
- Cross-check interfaces between subsystems next session.

</details>

---

<details>
<summary>Actions Agreed</summary>

- **All members:** Finalise Task 3 commits.  
- **All members:** Prepare microservice list (provided + required).  
- **All members:** Create initial Task 4a component diagram draft.  
- **All members:** Make at least one GitHub commit for Task 4 this week.  
- **All members:** Continue referring to case study + lecture notes.  
- **Next Meeting:** Tuesday 11/11/25 at 14:00.  

</details>

---

<details>
<summary>Issues Raised</summary>

- Papyrus performance slow — continue using alignment + properties panel.
- Emphasis on avoiding commit history loss when moving files.
- Clarifying microservice granularity — start simple and refine.

</details>

---

**Prepared by:** Areebah  
**Date of Writing:** 04/11/25  
