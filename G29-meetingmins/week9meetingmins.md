# COMP5047 Applied Software Engineering  
## Group G29 – Week 9 Meeting Agenda & Minutes  

**Date:** 19/11/25  
**Time:** 15:00 - 16:00  
**Location:** Google Meet  

**Attendees:**  
- David Gaman (19238600)  
- Aziz Hussein Boakye (19067039)  
- Areebah Khan (19343387)  
- Daniil Tkachenko (19323083)  

All Present  

---

## Agenda

1. Final review of Task 4(a) subsystem architectural designs.  
2. Begin Task 4(b) – integration of subsystem architectures into full system design.  
3. Cross-check interface naming, merging equivalent components, and resolving conflicts.  
4. Review Week 8 and Week 9 lecture content (structural + behavioural design).  
5. Plan Task 5(a): class diagram development for individual microservices.  
6. Discuss expectations for Task 5(b): sequence diagrams.  
7. Review GitHub activity, folder consistency, and incremental commits.  

---

<details>
<summary>Progress Since Last Meeting</summary>

- All members finalised their **Task 4(a)** subsystem component diagrams after applying corrections from Week 8.  
- Provided + required interfaces now consistently named (e.g., `IEventManagement`, `IUnionMembershipGateway`).  
- All microservices now follow the agreed naming structure (`*Service`, `*Gateway`, `*Adapter`).  
- Everyone reviewed Week 8 lecture content on **UML class diagrams** in preparation for Task 5(a).  
- Multiple GitHub commits completed across `/uml/task4/` and `/docs/task4/`.  
- Continued active communication over WhatsApp: sharing screenshots, diagrams, and clarifying interface dependencies.

</details>

---

<details>
<summary>Key Decisions</summary>

- Task 4(a) is considered **complete for all members**. Minor textual documentation edits remain but the diagrams are final.  
- The team will now start **Task 4(b)**—the integrated whole-system architectural design.  
- If two subsystems expose the same functionality, the interface will be **merged** during integration.  
- If components share the same name but different functionality, the team will **rename them for clarity** (per Week 9 coursework instructions).  
- Each member will begin **Task 5(a) Class Diagram** for one microservice within their subsystem boundary.  
- Class diagrams must follow principles covered in lectures:  
  - high cohesion  
  - precise associations  
  - lifecycle relationships  
  - consistency with microservice boundaries  
- Sequence diagrams in Task 5(b) must reflect the internal behaviour of *that same* microservice.

</details>

---

<details>
<summary>Discussion</summary>

### Final Review of Task 4(a)

- **Areebah** presented her refined USU Operation component model and said:  
  > “I made sure all the approval workflows clearly show which subsystem they depend on. The interfaces now exactly match the case study semantics.”

- **Aziz** demonstrated the Student Union Management subsystem updates:  
  > “I split the big approval component because it was doing too much. Now the services are more focused and the required interfaces are much cleaner.”

- **David** reviewed his Student App subsystem:  
  > “I added the method names under each interface because it makes the diagram look more complete. The gateway pattern now isolates all cloud interactions.”

- **Daniil** walked through his Society Leader subsystem:  
  > “I cleaned up the event management service and made sure it interacts consistently with both the union and USU services.”

The team confirmed all subsystem diagrams now align in style, structure, and naming.

---

### Starting Task 4(b) – Whole-System Integration

- A shared Papyrus file will be used to combine all subsystem diagrams using separate packages.  
- The team agreed the integrated diagram will show:  
  - four subsystem boundaries  
  - internal microservices  
  - all required/provided interfaces  
  - shared components merged into a single authoritative version

- **David** highlighted:  
  > “If two subsystems expose the same operations, we can’t show them twice—otherwise it breaks the microservice model.”

- **Aziz** added:  
  > “Let’s also mark which interfaces represent synchronous calls and which might be notifications. We don’t need all details, but the direction matters.”

The group will aim for a first full integration draft before Week 10.

---

### Preparation for Task 5(a) – Class Diagram

Each member selected one internal microservice:

- **Areebah:** `UnionMembershipService`  
- **Aziz:** `SocietyApprovalService`  
- **David:** `StudentProfileService`  
- **Daniil:** `SocietyEventService`  

Guidelines agreed:

- Show only classes inside the microservice boundary.  
- Use types consistent with entity names across subsystems.  
- Ensure each operation in the class diagram corresponds to an interface method defined in Task 4(a).  
- Include associations (e.g., 1..*, optional, composition) where appropriate.

**Areebah** noted:  
> “The case study shows how structural and behavioural models expose mistakes, so we need to be ready to revise the class diagrams later.”

---

### Planning for Task 5(b) – Behavioural Design

- The team reviewed the Week 9 lecture examples for sequence diagrams.  
- Diagrams should model **internal behaviour only** (not cross-subsystem communication).  
- Alternate/optional frames required for branching operations.  
- The team may revise Task 5(a) if 5(b) reveals inconsistencies.

**Daniil** said:  
> “My class diagram might need an operations split once I start the sequence diagram, but I won’t know until I model the actual behaviour.”

---

### GitHub & Workflow

- Directory structure confirmed:  
  -  subsystem & integrated component diagrams  
  - class + sequence diagrams  
  -  textual documentation for architectural components  

- Incremental commits encouraged.  
- **Areebah** reminded the team:  
  > “Please don’t re-upload the same file as new. Use rename or move inside GitHub so we keep commit history intact.”

</details>

---

<details>
<summary>Actions Agreed</summary>

- **All members:** Begin Task 5(a) class diagrams for chosen microservices.  
- **Group:** Start building the shared whole-system architectural model (Task 4b).  
- **All members:** Complete textual documentation for microservices defined in 4(a).  
- **All members:** Review Week 9 behavioural modelling lecture to prepare for Task 5(b).  
- **All members:** Make at least one GitHub commit before next meeting.  
- **Next Meeting:** Tuesday 25/11/25 at 17:00.  

</details>

---

<details>
<summary>Issues Raised</summary>

- Minor inconsistencies in naming (capitalisation, camelCase vs PascalCase) still need alignment in a shared glossary.  
- Integration diagram may become visually complex the team agreed to use subsystem packages to keep clarity.  
- Papyrus continues to lag; frequent saves recommended.  
- Class diagrams may expose gaps in interface method definitions, requiring updates to 4(a).  
- Need to ensure members do not accidentally model cross-microservice logic inside their class diagrams.

</details>

---

**Prepared by:** Areebah  
**Date of Writing:** 18/11/25  
