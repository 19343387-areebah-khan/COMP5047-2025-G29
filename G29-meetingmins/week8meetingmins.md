# COMP5047 Applied Software Engineering  
## Group G29 – Week 8 Meeting Agenda & Minutes  

**Date:** 11/11/25  
**Time:** 15:00–17:00  
**Location:** Google Meet  

**Attendees:**  
- David Gaman (19238600)  
- Aziz Hussein Boakye (19067039)  
- Areebah Khan (19343387)  
- Daniil Tkachenko (19323083)  

All Present  

---

## Agenda

1. Review each other's initial Task 4a drafts (microservices architectural design).  
2. Check consistency of interfaces, naming conventions, and subsystem boundaries.  
3. Clarify expectations for finalising microservice lists + component diagrams.  
4. Discuss lecture content on microservice architecture and how it applies.  
5. Review GitHub commits and ensure files are stored in correct folders.  
6. Plan what needs completing before Week 9 (integration stage / Task 4b prep).  

---

<details>
<summary>Progress Since Last Meeting</summary>

- All members have started Task 4a and produced a first draft of subsystem microservice diagrams.  
- Rough microservice lists completed, including provided and requested services.  
- Consistent messaging on WhatsApp, sharing screenshots and notes.  
- Reviewed Week 7/8 architectural lecture notes to match expected microservice structure.  
- All members have committed at least once for Task 4a.

</details>

---

<details>
<summary>Key Decisions</summary>

- Continue refining Task 4a diagrams, ensuring clear subsystem boundaries and APIs.  
- Use consistent naming conventions: `*Service`, `*Gateway`, `*Adapter`, `I*Interface`.  
- Each diagram should show internal microservices, provided interfaces, and required interfaces.  
- Only show method names for now — parameters will be added in the textual docs later.  
- Agree shared entity names (e.g. `UnionId`, `StudentId`, `SocietyId`, `EventId`).  
- Finalise first full draft of Task 4a by next meeting so Task 4b (system integration) can begin.  

</details>

---

<details>
<summary>Discussion</summary>

### Review of Task 4a Drafts
- Each member briefly presented their draft UML component diagram.  
- **Areebah** highlighted subsystem structure for USU Operation, including approval workflows and federation services.  
- **Aziz** showed the Student Union Management subsystem focusing on society and event approval flows.  
- **David** presented student-facing services, confirming gateway pattern for event and user requests.  
- **Daniil** outlined society management and event creation processes with union interaction points.  

Everyone agreed the diagrams are aligned with the case study and requirements.

### Microservices + Interfaces
- Verified initial microservice lists follow architectural style (bounded context, separation of concerns).  
- Confirmed each subsystem exposes APIs and consumes others through a gateway/service port.  
- Agreed to annotate communication style where relevant (REST / internal API call / message broker future-fit).  

### Naming & Structure Consistency
- Maintain readability — avoid overly granular services.  
- Must ensure consistent naming for shared entities.  
- Avoid shared databases — microservices remain isolated.  

### GitHub & Workflow
- Files must be committed  
- Attempt incremental commits rather than uploading final files in one go.  
- Save Papyrus often due to performance issues.  

### Next Steps
- Add interface method stubs (e.g., `createEvent()`, `approveSociety()`).  
- Begin writing textual component descriptions as required by spec.  
- Prepare for cross-subsystem integration in Task 4b.  

</details>

---

<details>
<summary>Actions Agreed</summary>

- **All members:** Refine Task 4a component diagrams with final microservice lists.  
- **All members:** Document provided/required interfaces with method names.  
- **All members:** Commit updates to GitHub this week.  
- **All members:** Review architectural lecture notes again to align with marking criteria.  
- **Group:** Prepare to integrate subsystem designs in Week 9.  
- **Next Meeting:** Tuesday 18/11/25 at 17:00.  

</details>

---

<details>
<summary>Issues Raised</summary>

- Minor inconsistencies in interface naming , continue syncing glossary terms.  
- Papyrus performance issues — team continues applying layout and property panel techniques.  
- Need to keep checking each other's subsystem diagrams to ensure interface alignment.  
- Remain mindful of microservice isolation, no shared persistence.  

</details>

---

**Prepared by:** Areebah  
**Date of Writing:** 11/11/25  
