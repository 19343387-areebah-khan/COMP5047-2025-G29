# COMP5047 Applied Software Engineering  
## Group G29 – Week 4 Meeting Agenda & Minutes  

**Date:** 14/10/25  
**Time:** 15:00–16:30  
**Location:** Google Meet  

**Attendees:**  
- David Gaman (19238600)  
- Aziz Hussein Boakye (19067039)  
- Areebah Khan (19343387)  
- Daniil Tkachenko (19323083)  

All Present  

---

## Agenda

1. Review progress from Week 3 (use case models, activity diagram drafts, quality requirements, functional requirements documentation).  
2. Discuss principles of software modelling and UML activity diagrams.  
3. Cross-check each other’s Task 3(b) activity diagrams for correctness, consistency, and completeness.  
4. Discuss and clarify data sources needed for each subsystem to respond to users' requests:  
   - User input vs. system-stored data  
   - Which subsystem provides the data if it comes from the system  
5. Plan updates for GitHub repository with finalized Week 4 artefacts.  
6. Assign individual tasks for Week 5 (software architectural design).  

---

<details>
<summary>Progress Since Last Meeting</summary>

- Week 3 activity diagrams partially completed by all members in Papyrus.  
- Quality requirements document - some members still need to upload 
- Functional requirements documentation for each subsystem drafted and shared.  
- Peer review of initial activity diagram drafts completed informally via WhatsApp.  

</details>

---

<details>
<summary>Key Decisions</summary>

- Each member to finalize **Task 3(b) activity diagram** corresponding to a selected use case from their Week 3 use case model.  
- Explicitly mark data inputs in the activity diagrams as either **user input** or **system-stored data**.  
- Activity diagrams and functional requirements documents to be updated and uploaded to GitHub **by Friday 17/10/25**.  
- Papyrus confirmed as the standard UML tool to maintain consistency across subsystems.  

</details>

---

<details>
<summary>Discussion</summary>

- **Activity Diagrams:**  
  - Daniil: USU Student App activity diagram reviewed; decision nodes updated for event registration process. 
  - Aziz: Student Union Management System diagram reviewed; membership approval workflow clarified. He mentioned: "The approval should clearly show coming from the USU Operation System."  
  - Areebah: USU Operation System diagram reviewed; swimlanes added to show microservice responsibilities. 
  - David: Society Leader App diagram reviewed; clarified interactions with Student Union Management System for event approvals. He noted:  
    > "Event approval data comes from the Union Management microservice so diagrams need to acknowledge this."  

- **Data Dependencies:**  
  - Each subsystem reviewed required data for responses.  
  - Marked whether data comes from user input or system storage.  
  - Identified which subsystem provides stored data; to be documented in Week 5 architecture.  

- **GitHub Repository:**  
  - Group is not happy with the repo it is not organised that well areebah said she will try to improve it. 

- **Preparation for Week 5:**  
  - Focus on software architectural design using UML component diagrams in microservices style.  
  - Each member to review their use case and activity diagram before starting architectural design.  

</details>

---

<details>
<summary>Actions Agreed</summary>

- **All Members:** Finalize Task 3(b) activity diagram for their assigned subsystem, marking data sources.  
- **All Members:** Upload final activity diagrams and updated functional requirements to GitHub by **Friday 17/10/25**.  
- **Areebah:** Prepare guidelines for Week 5 architectural design, including component identification and API documentation.Still needs to upload task 3a.  
- **David:** Check repository structure and ensure all Week 4 artefacts are correctly placed.  
- **All Members:** Review each other’s activity diagrams for consistency and correctness before final GitHub commit.  
- **Next Meeting:** Week 5 on Tuesday 21/10/25, 15:00.  

</details>

---

<details>
<summary>Issues Raised</summary>

- Papyrus occasionally has save/export issues: frequent GitHub commits recommended.  
- Minor uncertainties on swimlane placement and decision nodes: peer review to resolve.  
- Ambiguity on inter-subsystem data flow: to be clarified in Week 5 architecture task.
- May need to change the GitHub repo layout still not sure the best way to display and organise it - Areebah will look into this. 

</details>

---

**Prepared by:** Areebah  
**Date of Writing:** 14/10/25  
