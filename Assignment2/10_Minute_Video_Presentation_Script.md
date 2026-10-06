# COIT20270 Assignment 2: 10-Minute Video Presentation Script
## Turn-Key Speaker Guide & Live Demonstration Blueprint

**Student Author:** Sadiq Salman (Student ID: 12284952)  
**Course:** COIT20270 App Development for Mobile Platforms — CQUniversity Australia  
**Assignment:** Assignment 2 Prototype (30%)  
**Application:** ElegantLink — Client Governance Mobile Platform (Elegant Media Australia)  
**Total Target Video Duration:** Exactly 10 Minutes (600 Seconds)  
**Submission Format:** Video recording submitted via CQU OneDrive shared link  

---

## Technical Recording Setup Checklist

Before recording your screen and webcam (e.g., using OBS Studio, Zoom, or Microsoft Teams):
1. **DartPad Preparation:** Open [dartpad.dev](https://dartpad.dev) in your web browser. Paste the complete code from `Assign2/lib/main.dart` into the editor and click **Run**. Verify that the app renders without any compilation errors.
2. **Window Sizing:** Start with the DartPad preview pane sized to a mobile aspect ratio (width $<640\text{dp}$, approximately $390\text{px}$ wide) to showcase the mobile layout.
3. **Slide Deck:** Open `Assign2/Assignment2_Presentation_Deck.pptx` in presenter view or full screen on a secondary monitor or split screen.
4. **Microphone & Lighting:** Ensure your audio is clear and webcam is positioned in the upper or lower corner without obstructing critical slide content.

---

## Detailed Minute-by-Minute Script & Cue Cards

```
================================================================================
PART 1: INTRODUCTION & PROBLEM EVOLUTION (0:00 – 1:50)
================================================================================
```

### [0:00 – 0:30] Slide 1: Title & Presentation Overview
* **Visual on Screen:** Slide 1 (Title Slide: Candidate Metadata, Assessment Details, Deliverable Links)
* **Presenter Action:** Speak clearly with professional enthusiasm; webcam visible.
* **Spoken Dialogue:**
  > "Hello and welcome. My name is Sadiq Salman, student ID 12284952. Welcome to my Assignment 2 Prototype presentation for COIT20270: App Development for Mobile Platforms at Central Queensland University. 
  > 
  > Today, I am proud to present the working Flutter prototype of ElegantLink, a dedicated client governance mobile application engineered for Australian software development consultancy Elegant Media. Over the next ten minutes, I will guide you through our system problem statement, our empirical persona Founder Fred, our UML and Activity Diagram walkthroughs with live app demonstrations on DartPad, our canonical Material 3 responsive architecture, mobile heuristics evaluation, privacy governance, and code-level design."

---

### [0:30 – 1:10] Slide 2: Transitioning from System Design to Interactive Prototype
* **Visual on Screen:** Slide 2 (Problem Statement, Opacity, Jargon, and Working Prototype Solution)
* **Spoken Dialogue:**
  > "In Assignment 1, we identified the fundamental operational problem facing Elegant Media: following commercial agreement and payment of an initial financial deposit, software clients enter an informational black box. Development progress is communicated through sporadic email chains saturated with technical software engineering terms—such as Git pull requests, API schema modifications, and sprint burndowns—which non-technical business founders cannot evaluate. 
  > 
  > This industry friction is well documented in academic literature. Zhao et al. (2024, page 2084) establish that software project measurement requires structured, transparent indicators so non-technical stakeholders can monitor quality through objective measurement rather than subjective reassurance. In Assignment 2, we have translated our conceptual models into a fully operational Material 3 Flutter prototype that resolves this void."

---

### [1:10 – 1:50] Slide 3: Persona: Founder Fred (Fred R.)
* **Visual on Screen:** Slide 3 (Founder Fred Profile, Technostress & Outdoor Contrast Needs)
* **Spoken Dialogue:**
  > "Every design choice in our prototype was shaped by our empirical persona, Founder Fred—standardized throughout our interface as Fred R. Fred is a 42-year-old managing director of a retail business in Melbourne who commissioned custom software. He checks his phone in brief 10 to 60-second micro-breaks between warehouse inspections and client meetings.
  > 
  > Wang and Yu (2024, page 3) observed that 'technostress has a direct negative impact on user satisfaction and continuance intention to use mobile applications.' Exposing Fred to raw developer tools like Jira induces technostress, leading to disengagement. Furthermore, Punsongserm and Suvakunta (2025, page 21) demonstrated that mobile readability collapses under bright outdoor illumination unless minimum contrast standards are met. Consequently, ElegantLink strictly enforces WCAG 2.1 AA high contrast, large touch targets, and jargon-free summaries."

---

```
================================================================================
PART 2: ARCHITECTURE & USE CASE WALKTHROUGHS (1:50 – 5:35)
================================================================================
```

### [1:50 – 2:25] Slide 4: UML Use Case Diagram (UCD)
* **Visual on Screen:** Slide 4 (Figure 1: Use Case Diagram with System Boundary)
* **Spoken Dialogue:**
  > "Slide 4 shows our UML Use Case Diagram, structured around actor goals rather than UI procedural steps. The system boundary clearly separates external client Fred R. from Elegant Media Project Manager James R. 
  > 
  > Fred interacts with four primary capabilities: viewing curated project status, reviewing uploaded artefacts and giving contextual feedback, approving milestones or requesting revisions, and managing data privacy consent. On the agency side, James curates sanitized updates and records formal governance decisions. Notice that 'Manage Privacy and Consent' is elevated as a primary use case, upholding Fred's data sovereignty."

---

### [2:25 – 3:25] Slide 5 + LIVE APP DEMO 1: Activity Diagram 1 & Status Walkthrough
* **Visual on Screen:** Slide 5 (Figure 2: Activity Diagram 1) $\rightarrow$ **[SWITCH TO DARTPAD PREVIEW]**
* **Presenter Action:** 
  1. Show Slide 5 briefly (15 seconds), pointing out Client vs Service swimlanes.
  2. Switch screen to the live DartPad app preview running on mobile view.
* **Spoken Dialogue:**
  > "Activity Diagram 1 models how Fred inspects project status. The diagram uses distinct swimlanes for Client and ElegantLink Service. When Fred launches the app, background authentication occurs automatically, rendering the ambient dashboard.
  > 
  > Let's look at this live in our running app on DartPad. **[Point mouse to Dashboard Screen]**
  > Fred is immediately greeted with an ambient health card—currently green for 'On Track'—showing his active project, Stage 3 Core UI Screens at 65% completion, and a prominent 'Next Required Action' banner alerting him to review a deliverable. 
  > 
  > Following the alternative decision branch in Activity Diagram 1, if Fred is in a rush, he can glance and close the app in under ten seconds. But if he requires further details, he simply taps the active stage card **[Tap on Core UI Screens card]**, navigating to the 5-Stage SDLC Detail Screen, where he can inspect plain-language stage milestones with exact completion percentages."

---

### [3:25 – 4:30] Slide 6 + LIVE APP DEMO 2: Activity Diagram 2 & Feedback Loop
* **Visual on Screen:** Slide 6 (Figure 3: Activity Diagram 2) $\rightarrow$ **[SWITCH TO DARTPAD PREVIEW]**
* **Presenter Action:**
  1. Return to Slide 6 for 15 seconds to explain the verified discard logic in AD2.
  2. Switch to DartPad: Navigate to Projects Tab, open Deliverables, tap a mockup, type a test comment, and demonstrate discard vs submit.
* **Spoken Dialogue:**
  > "Activity Diagram 2 details deliverable review and contextual feedback, implemented across Screens 5 and 6. Crucially, AD2 features verified discard logic: selecting Cancel safely clears draft feedback, while selecting Submit logs an audit timestamp and notifies the project manager.
  > 
  > In our live prototype, Fred taps the Projects tab in the bottom NavigationBar **[Tap Projects]**. He selects the 'Deliverables' tab at the top **[Tap Deliverables]**, which displays a filterable gallery of UI mockups. Tapping on 'Mobile Checkout Flow v2.1' **[Tap card]** opens the Mockup Viewer. 
  > 
  > Notice the anchored discussion thread directly beneath the image: James R. posted the initial deliverable, and Fred replied. If Fred types a comment into the input field **[Type: 'Looks good, please verify the card layout']** and hits the Clear button, the draft safely clears. When he hits Send **[Tap Send Icon]**, the comment appends to the thread with an audit timestamp and displays a Material 3 confirmation SnackBar."

---

### [4:30 – 5:35] Slide 7 + LIVE APP DEMO 3: Activity Diagram 3 & Milestone Sign-Off
* **Visual on Screen:** Slide 7 (Figure 4: Activity Diagram 3) $\rightarrow$ **[SWITCH TO DARTPAD PREVIEW]**
* **Presenter Action:**
  1. Show Slide 7 (15 seconds) highlighting the two-step neutral confirmation and revision branches.
  2. Switch to DartPad: Tap Governance Tab, review the checklist and \$12,500 fee, tap 'Request Changes', return, tap 'Approve Milestone' to show the modal, confirm, and show the Digital Certificate.
* **Spoken Dialogue:**
  > "Activity Diagram 3 governs commercial milestone acceptance, implemented across Screens 7, 8, and 9. Milestone approvals carry binding financial liabilities, such as triggering milestone progress payments. Therefore, our flow implements a strict two-step confirmation process to prevent accidental taps.
  > 
  > Let's demonstrate this live. In our app, Fred taps the 'Governance' tab **[Tap Governance]**. He sees the milestone review for Stage 3, detailing the completed acceptance criteria and the commercial fee of \$12,500 AUD. 
  > 
  > Notice the equal visual weight of 'Approve Milestone' and 'Request Changes'—rejecting dark patterns. If Fred selects 'Request Changes' **[Tap Request Changes]**, he is taken to a structured revision form. 
  > 
  > If he selects 'Approve Milestone' **[Tap Approve Milestone]**, the app triggers a neutral secondary confirmation dialog that explicitly summarizes the legal and invoice liabilities. Once Fred confirms **[Tap Confirm Approval]**, the system records an immutable audit log and presents a cryptographically signed Digital Certificate with a SHA-256 hash, User ID, and timestamp."

---

```
================================================================================
PART 3: RESPONSIVE DEMO & GUIDELINES ADHERENCE (5:35 – 7:20)
================================================================================
```

### [5:35 – 6:35] Slide 8 + LIVE RESPONSIVE DEMO: Canonical Material 3 Layouts
* **Visual on Screen:** Slide 8 (Breakpoints: `<640dp` vs `\ge 640dp`) $\rightarrow$ **[SWITCH TO DARTPAD WINDOW RESIZE]**
* **Presenter Action:**
  1. Show Slide 8 for 10 seconds.
  2. Switch to the DartPad browser window.
  3. Start at narrow mobile width ($<640\text{dp}$). Point to the bottom `NavigationBar`.
  4. Slowly drag the browser / preview window resize handle wider until screen width crosses $640\text{dp}$.
  5. Show the bottom `NavigationBar` disappearing and the left `NavigationRail` dynamically appearing, with cards reflowing into a two-column grid.
* **Spoken Dialogue:**
  > "In compliance with Criterion 1, our prototype implements canonical Material 3 responsive layouts using Flutter's LayoutBuilder. 
  > 
  > Let's see this in action live right now. **[Point to DartPad Preview]**
  > In this mobile viewport under 640dp, the app utilizes a canonical bottom NavigationBar with filled active indicator pills, placing navigation within Fred's natural thumb zone for one-handed operation. 
  > 
  > Now, watch closely as I expand the preview window wider, simulating Fred opening the app on his iPad or desktop web browser **[Slowly drag window width past 640dp]**. 
  > 
  > The navigation dynamically transforms into an adaptive left NavigationRail, featuring permanent branding, extended destinations, and a settings action. Simultaneously, the content surface automatically reflows from a single column into an expansive, airy two-column grid using LayoutBuilder. There are no layout overflow errors or unbounded constraints. It adapts seamlessly across all viewport form factors."

---

### [6:35 – 7:20] Slide 9: Adherence to Material 3 UI Guidelines
* **Visual on Screen:** Slide 9 (Component Checklist: AppBar, NavBar, Rail, Tab, Carousel, List, Card, Form/TextField, Dialog, FAB, SnackBar)
* **Presenter Action:** Return to slide presentation; point out how each component adheres to official Material 3 specs.
* **Spoken Dialogue:**
  > "Slide 9 presents our detailed Material 3 component mapping matrix, demonstrating exhaustive adherence to every mandated widget in the unit rubric. 
  > 
  > In our AppBars, we implement centered titles with scrolled surface elevation tint. Our NavigationBar and NavigationRail employ filled active indicator pills with unbolded unselected states. Our TabBars utilize primary pill tabs with smooth animation. For content display, we use outlined Material 3 cards with subtle 1dp borders and 16dp rounded corners, strictly avoiding antipatterns like nesting ListViews inside cards. 
  > 
  > In deliverable review, we implement a PageController carousel with active dot indicators. Furthermore, our authentication and feedback flows implement Material 3 Forms and TextFormFields with RFC regex email validation. For feedback and overlays, we employ neutral AlertDialogs with equal-weight action buttons, extended Floating Action Buttons, non-intrusive SnackBars, and modal bottom sheets for privacy settings. Every touch target meets or exceeds the canonical 48 by 48dp accessibility standard."

---

```
================================================================================
PART 4: HEURISTICS, USABILITY GOALS & PRIVACY (7:20 – 9:15)
================================================================================
```

### [7:20 – 8:05] Slides 10 & 11: Static Mobile Heuristic Evaluation
* **Visual on Screen:** Slide 10 (Micro-Usage & Glanceability) $\rightarrow$ Slide 11 (Error Prevention & Consistency)
* **Spoken Dialogue:**
  > "Evaluating our prototype against static mobile heuristics reveals strong grounding in Fred's cognitive and physical environment. 
  > 
  > First, Quick Interaction and Micro-Usage: Fred operates in 10-to-60-second bursts. Our ambient dashboard surfaces overall project health and the next required action immediately upon launch, allowing Fred to glance and exit in under ten seconds. Ilany-Tzur and Fink (2023, page 2446) showed that dense data structures impair mobile user performance; our app eliminates developer jargon, reducing cognitive load. Gatsou et al. (2011, page 273) confirmed that visual metaphors accelerate novice recognition, which we implement via traffic-light badges.
  > 
  > Second, Error Prevention and Consistency: Milestone approvals trigger binding invoices; our deliberate two-step confirmation dialog completely prevents accidental touchscreen taps. All stakeholders adhere to a uniform naming format: Fred R. and James R. Finally, all typography meets WCAG 2.1 AA standards exceeding 4.5:1 contrast, ensuring complete readability under bright sunlight."

---

### [8:05 – 8:40] Slide 12: Usability Goals Verification
* **Visual on Screen:** Slide 12 (5 Usability Goals Mapped to Observable Behaviors for Assessment 3)
* **Spoken Dialogue:**
  > "Slide 12 maps our five usability goals from Assignment 1 to our working prototype and outlines the empirical testing protocols for Assessment 3. 
  > 
  > Goal 1, Learnability: cold app launch to verbal stage recognition in 10 seconds or less. Goal 2, Efficiency: submitting contextual feedback in 60 seconds or less—representing an observable 40% time reduction compared to fragmented email chains. Goal 3, Error Prevention: exactly zero accidental milestone approvals across 20 trials. Goal 4, Satisfaction: achieving an above-average System Usability Scale score of 68 or higher. And Goal 5, Accessibility: full layout stability at 200% font scaling and WCAG AA contrast under simulated glare."

---

### [8:40 – 9:15] Slides 13, 14 & 15: Privacy Architecture & Ethical Design
* **Visual on Screen:** Slide 13 (DFD) $\rightarrow$ Slide 14 (APPs & CASFUD) $\rightarrow$ Slide 15 (Rejecting Dark Patterns)
* **Spoken Dialogue:**
  > "Our privacy architecture, shown in our Data Flow Diagram on Slide 13, strictly operationalizes the Australian Privacy Principles and the CASFUD framework. 
  > 
  > In accordance with LaMonica et al. (2021, page 5), who proved that dense legalistic policies destroy informed consent, ElegantLink uses plain-English in-app consent sheets with unbundled opt-in toggles. On the security front, Dahiya et al. (2024, page 3) emphasized defense-in-depth against mobile data interception; all data uses TLS 1.3 in transit and AES-256 at rest in Australian sovereign cloud facilities, with biometric authentication. Furthermore, diagnostic telemetry is stripped of all personal identity before storage.
  > 
  > Finally, on Slide 15, we actively repudiate mobile dark patterns. Li et al. (2025, page 8) documented how deceptive patterns manipulate users through asymmetric buttons and false urgency. In ElegantLink, 'Approve' and 'Request Changes' feature identical visual weight, countdown timers are prohibited, and exact financial fees are disclosed upfront."

---

```
================================================================================
PART 5: CODE WALKTHROUGH, INTEGRITY & CONCLUSION (9:15 – 10:00)
================================================================================
```

### [9:15 – 9:45] Slide 16 + CODE WALKTHROUGH: Code-Level Screen Design & Software Architecture
* **Visual on Screen:** Slide 16 $\rightarrow$ **[SWITCH TO DARTPAD CODE EDITOR / VS CODE]**
* **Presenter Action:**
  1. Show Slide 16 briefly (10 seconds).
  2. Switch to the DartPad code editor tab.
  3. Scroll through `main.dart`, highlighting the `ThemeData`, `AppStateModel` ChangeNotifier + `AppStateScope` InheritedNotifier reactive state architecture (including simulated authentication session), `LayoutBuilder` responsive shell, and rich design-level docstring comments.
* **Spoken Dialogue:**
  > "Slide 16 details our software architecture. In accordance with unit specifications, our prototype is packaged into a single, self-contained Dart file of 3,151 lines that compiles cleanly on dartpad.dev without external packages. 
  > 
  > Looking at the code in DartPad **[Scroll through code in editor]**, we implemented a clean reactive architecture using AppStateModel—extending ChangeNotifier—and AppStateScope—extending InheritedNotifier. This provides O(1) state lookups and automated widget rebuilds across all 11 screens, including our simulated authentication gate, with zero third-party dependencies. Our codebase is structured across six clear architectural tiers, from domain models up to dedicated screen widgets. 
  > 
  > Most importantly, complying with Criterion 3, our code is richly annotated with design-level comments explaining widget choices, persona alignment, touch targets, and heuristic principles, rather than trivial syntax descriptions."

---

### [9:45 – 10:00] Slides 17, 18 & 19: AI Collaboration, References & Conclusion
* **Visual on Screen:** Slide 17 $\rightarrow$ Slide 18 $\rightarrow$ Slide 19 (Submission Links & Conclusion)
* **Presenter Action:** Speak concluding remarks warmly; display submission links.
* **Spoken Dialogue:**
  > "Slide 17 discloses our use of Generative AI as an assistive peer-review tool, with all code, architectural flows, and citations personally verified by myself. Slide 18 presents our nine peer-reviewed journal articles from the CQU Library, complete with verbatim quotes and page numbers embedded in the slide notes. 
  > 
  > In conclusion, ElegantLink demonstrates an adaptive, canonical Material 3 prototype that brings transparency, speed, and peace of mind to commercial software clients. All submission links—including our DartPad code, private GitHub repository, and video link—are displayed on Slide 19. Thank you for your time and guidance."

---

## Quick-Glance Cue Cards for Presentation

| Timestamp | Screen State | Primary Spoken Cue / Action |
| :---: | :--- | :--- |
| **0:00** | Slide 1 (Title) | State name, ID (12284952), unit (COIT20270), and app concept (ElegantLink). |
| **0:30** | Slide 2 (Problem) | Explain post-deposit opacity, technical jargon, and Zhao et al. (2024). |
| **1:10** | Slide 3 (Persona) | Introduce Founder Fred (Fred R.), technostress (Wang & Yu), sunlight (Punsongserm). |
| **1:50** | Slide 4 (UCD) | Explain technology-agnostic governance boundary and external actor roles. |
| **2:25** | Slide 5 $\rightarrow$ **DartPad Preview** | **DEMO 1:** Show ambient dashboard, traffic-light badge, tap active stage to show 5-stage SDLC breakdown. |
| **3:25** | Slide 6 $\rightarrow$ **DartPad Preview** | **DEMO 2:** Navigate to Projects $\rightarrow$ Deliverables, open Mockup Viewer, show live thread, demo cancel vs submit. |
| **4:30** | Slide 7 $\rightarrow$ **DartPad Preview** | **DEMO 3:** Open Governance tab, show \$12,500 fee, demo neutral confirmation dialog, show signed Digital Certificate. |
| **5:35** | Slide 8 $\rightarrow$ **Window Resize** | **RESPONSIVE DEMO:** Start at mobile ($<640$dp) showing bottom `NavigationBar`; drag window wider ($>640$dp) to show left `NavigationRail` and 2-column reflow! |
| **6:35** | Slide 9 (M3 Checklist) | Walk through canonical M3 components: AppBar, NavBar, Rail, Tab, Card, Form/TextField, Dialog, FAB, SnackBar. |
| **7:20** | Slides 10 & 11 (Heuristics) | Explain micro-usage, glanceability, cognitive load, error prevention, uniform naming (Fred R. & James R.). |
| **8:05** | Slide 12 (Usability Goals) | Reiterate 5 observable behavioral goals for Assessment 3 (Learnability $\le 10$s, Efficiency $\le 60$s, etc.). |
| **8:40** | Slides 13–15 (Privacy/Ethics) | Walk through DFD (P1.0–P5.0), APPs/CASFUD compliance, and rejection of dark patterns (equal visual weight). |
| **9:15** | Slide 16 $\rightarrow$ **DartPad Code** | **CODE WALKTHROUGH:** Show single-file `main.dart` (3,151 lines), simulated auth gate, `LayoutBuilder`, canonical M3 APIs, and design comments. |
| **9:45** | Slides 17–19 (Wrap-up) | AI collaboration statement, 9 CQU library references, submission links, and closing thank you. |
