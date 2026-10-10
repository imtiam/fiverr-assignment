# COIT20270 Assignment 3: Participant Testing Protocol & Facilitator Scripts
## Usability Goals Empirical Evaluation for "ElegantLink"

**Unit:** COIT20270 App Development for Mobile Platforms (CQUniversity Australia)  
**Assessment:** Assignment 3 — Usability Goals  
**Investigator:** Sadiq Salman (Student ID: 12284952)  
**Prototype Runtime:** Flutter Material 3 Single-File Engine on [dartpad.dev](https://dartpad.dev)  
**Target User Persona:** Founder Fred (Fred R., Age 42, Managing Director, Non-Technical)  

---

## 1. Participant Recruitment Profiles

In compliance with the Assignment 3 rubric, three (3) diverse participants were recruited to provide balanced, comprehensive usability data:

| Participant ID | Demographic Profile | Persona Alignment | Device Environment | Testing Role & Rationale |
| :--- | :--- | :--- | :--- | :--- |
| **Participant 1 (P1)** | Male, Age 44, Managing Director of an Australian retail enterprise | **Primary Persona Match ("Founder Fred"):** Non-technical executive, time-poor, anxious regarding project drift and commercial liability. | Mobile Viewport (412 $\times$ 915dp, Touch Screen) | Evaluates whether executive glanceability, anti-technostress design, and commercial liability clarity resonate with the target persona. |
| **Participant 2 (P2)** | Female, Age 38, Operations Coordinator in logistics | **Novice Client Match:** Non-technical consumer, unfamiliar with Jira/GitHub or software terminology, relies on clear affordances. | Mobile Viewport (390 $\times$ 844dp, Smartphone) | Evaluates intuitive learnability, cognitive friction in design review, and vulnerability to accidental confirmation errors. |
| **Participant 3 (P3)** | Male, Age 23, Final-year undergraduate computing student | **Peer / Technical Reviewer Match:** Digitally literate, experienced with mobile UI paradigms, critical of UX polish and edge cases. | Tablet / Desktop Viewport (1024 $\times$ 768dp, Desktop Browser) | Evaluates responsive layout transitions (NavigationRail vs NavigationBar), input validation speed, and interface stability. |

---

## 2. The Three Usability Goals & Associated Tasks

The three tasks tested across all three participants map directly to the pre-defined usability goals in Section 6 of the Assignment 1 specification:

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                        USABILITY GOAL & TASK MAPPING ARCHITECTURE                      │
├────────────────────────────┬───────────────────────────────────────────────────────────┤
│ Task 1 (Learnability)      │ Goal 6.1: Ambient status & stage recognized in <=10s      │
│ Target Screen: Screen 2    │ Activity Diagram 1: View Project Status                   │
├────────────────────────────┼───────────────────────────────────────────────────────────┤
│ Task 2 (Efficiency)        │ Goal 6.2: Contextual deliverable feedback in <=60s        │
│ Target Screen: Screen 6    │ Activity Diagram 2: Review Artefact & Submit Feedback     │
├────────────────────────────┼───────────────────────────────────────────────────────────┤
│ Task 3 (Error Prevention)  │ Goal 6.3: 0 unintended milestone approvals; 100% liability│
│ Target Screen: Screen 7    │ Activity Diagram 3: Approve Milestone or Request Changes │
└────────────────────────────┴───────────────────────────────────────────────────────────┘
```

### Task 1 Specification: Cold Launch & Ambient Status Identification
* **Associated Usability Goal:** Usability Goal 6.1 (Learnability).
* **Assignment 1 Baseline Benchmark:** Time-on-task $\le 10$ seconds from cold app launch; $\ge 90\%$ verbal recognition accuracy of current phase and project health.
* **Scholarly Grounding:** Gatsou et al. (2011, p. 275) prove that visual metaphors and high-contrast badges accelerate novice comprehension under executive time pressure.
* **Task Scenario Prompt given to Participant:**  
  > *"Imagine you are Founder Fred opening the app between business meetings. Launch the app, enter the executive demo credentials, and tell me: what is the current development phase of your Retail Ordering App, and is the project currently on schedule?"*
* **Success Criteria:** Participant identifies **"Stage 3: Core Implementation"** and **"ON SCHEDULE / HEALTHY"** without consulting any documentation.
* **Quantitative Metrics Recorded:** Elapsed time from dashboard display to correct verbal response (seconds); number of incorrect taps or hesitations.

---

### Task 2 Specification: Review Wireframe Deliverable & Submit Feedback
* **Associated Usability Goal:** Usability Goal 6.2 (Efficiency).
* **Assignment 1 Baseline Benchmark:** Contextual feedback submitted in $\le 60$ seconds (achieving a $\ge 40\%$ reduction compared to fragmented email chains).
* **Scholarly Grounding:** Jakob et al. (2022, p. 8) demonstrate that anchoring feedback threads directly to visual design artefacts eliminates cognitive context switching.
* **Task Scenario Prompt given to Participant:**  
  > *"You received a notification from project manager James R. asking you to review the Cart & Checkout Wireframe mockup. Navigate to the Deliverables Gallery, open the mockup, inspect the ongoing discussion, and submit a brief comment or use a quick feedback chip to request a review of the payment gateway."*
* **Success Criteria:** Participant successfully opens Screen 6 (`MockupViewerScreen`), reads the existing comment thread, and posts a new comment (either using 1-tap quick chips or text input) that appears in the live audit list.
* **Quantitative Metrics Recorded:** Total elapsed time (seconds); number of taps required; navigation errors or wrong menu selections.

---

### Task 3 Specification: Milestone Commercial Governance & Approval Gate
* **Associated Usability Goal:** Usability Goal 6.3 (Error Prevention).
* **Assignment 1 Baseline Benchmark:** Accidental sign-off rate of exactly **0%**; 100% verbal awareness of the commercial payment liability (\$12,500 AUD inc. GST) prior to binding commitment.
* **Scholarly Grounding:** Li et al. (2025) and Jakob et al. (2022) prove that high-stakes commercial commitments must avoid dark patterns and enforce a deliberate two-step confirmation gateway.
* **Task Scenario Prompt given to Participant:**  
  > *"The agency has completed Milestone 2 and submitted it for formal sign-off. Navigate to Milestone 2 Governance, verify the completed acceptance criteria, find the commercial financial liability, and complete the sign-off process."*
* **Success Criteria:** Participant navigates to Screen 7 (`MilestoneSummaryScreen`), verbally acknowledges the \$12,500 AUD liability, taps 'Approve Milestone', reviews the confirmation dialog, and reaches the sealed digital certificate (`MilestoneApprovedScreen`).
* **Quantitative Metrics Recorded:** Slip rate (accidental taps outside the button); cancellation rate in dialog; verbal confirmation of \$12,500 AUD figure; elapsed time to certificate generation.

---

## 3. Step-by-Step Facilitator Script (For Video Recording)

### Step 1: Pre-Test Setup & Verbal Informed Consent (2 Minutes)
1. Verify screen recorder and microphone are active.
2. Ensure [dartpad.dev](https://dartpad.dev) is preloaded with `Assign3/main.dart` at the `LoginScreen`.
3. Read the standardized consent script:
   > **Facilitator:** *"Welcome [Participant Name]. Today we are conducting a usability test for CQUniversity assessment COIT20270. As outlined in the Information Sheet, your participation is voluntary, anonymous (coded as Participant [1/2/3]), recorded solely for CQU marking staff, and you can stop at any time. Do you confirm your informed consent?"*  
   > **Participant:** *"Yes, I confirm."*

### Step 2: Test Administration — Concurrent Think-Aloud (15 Minutes)
Instruct the participant to "think aloud" as they perform each task:
> **Facilitator:** *"Please speak your thoughts aloud as you interact with the app. Tell me what you are looking for, what you expect to happen, and if anything feels confusing or surprising. I will observe silently and only prompt you if necessary."*

* **Execute Task 1:** Present Task 1 prompt $\rightarrow$ Start stopwatch upon dashboard render $\rightarrow$ Stop stopwatch upon verbal identification of phase & health $\rightarrow$ Log time and observations.
* **Post-Task 1 Single Ease Question (SEQ):**  
  > *"On a scale of 1 to 7, where 1 is very difficult and 7 is very easy, how easy was it to find the project status?"*
* **Execute Task 2:** Present Task 2 prompt $\rightarrow$ Start stopwatch upon first tap $\rightarrow$ Stop stopwatch when comment appears in thread $\rightarrow$ Log time and observations.
* **Post-Task 2 Single Ease Question (SEQ):**  
  > *"On a scale of 1 to 7, how easy was it to inspect the wireframe and submit your feedback?"*
* **Execute Task 3:** Present Task 3 prompt $\rightarrow$ Start stopwatch $\rightarrow$ Observe interaction with dialog and liability card $\rightarrow$ Stop stopwatch upon certificate generation $\rightarrow$ Log time and slip occurrences.
* **Post-Task 3 Single Ease Question (SEQ):**  
  > *"On a scale of 1 to 7, how easy was it to review the milestone criteria and complete the sign-off?"*

### Step 3: Post-Test Debriefing & Qualitative Feedback (3 Minutes)
Ask three open-ended reflective questions:
1. *"What was the most intuitive or helpful feature in the app?"*
2. *"Where did you feel any hesitation or uncertainty?"*
3. *"If you were Founder Fred managing a \$50,000 project, what additional control or feature would give you greater confidence?"*
4. Thank the participant and conclude the video recording.
