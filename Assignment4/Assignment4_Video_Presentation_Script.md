# COIT20270 Assignment 4: 10-Minute Video Presentation Script
## Turn-Key Speaker Guide & Live Demonstration Blueprint

**Student Author:** Sadiq Salman (Student ID: 12284952)  
**Course:** COIT20270 App Development for Mobile Platforms — CQUniversity Australia  
**Assignment:** Assignment 4 Practical (30%)  
**Application:** ElegantLink — Production Client Governance Mobile Platform (Elegant Media Australia)  
**Total Target Video Duration:** Exactly 10 Minutes (600 Seconds)  
**Submission Format:** Video recording submitted via CQU OneDrive shared link  

---

## Technical Recording Setup Checklist

Before recording your screen and webcam (e.g., using OBS Studio, Zoom, or Microsoft Teams):
1. **DartPad Preparation:** Open [dartpad.dev](https://dartpad.dev) in your web browser. Paste the complete code from `Assign4/main.dart` (3,633 lines) into the editor and click **Run**. Verify that the app compiles and renders without errors.
2. **Window Sizing for Demos:** Start with the DartPad preview pane sized to a mobile viewport (width $<640\text{dp}$, approximately $390\text{px}$ wide) to showcase the phone layout.
3. **Slide Deck:** Open `Assign4/Assignment4_slides.pptx` in presenter view on a secondary monitor or split screen.
4. **Deployed PWA:** Have your live PWA link open in a browser tab ready to demonstrate mobile web installation.
5. **Microphone & Webcam:** Ensure clear audio and webcam positioning that does not obstruct slide content.

---

## Detailed Minute-by-Minute Script & Cue Cards

```
================================================================================
PART 1: INTRODUCTION, PROBLEM & ARCHITECTURAL FOUNDATIONS (0:00 – 1:40)
================================================================================
```

### [0:00 – 0:35] Slide 1: Title & Presentation Overview
* **Visual on Screen:** Slide 1 (Title Slide: Candidate Metadata, Assessment Details, Deliverable Links)
* **Presenter Action:** Speak clearly with professional enthusiasm; webcam visible.
* **Spoken Dialogue:**
  > "Hello and welcome. My name is Sadiq Salman, student ID 12284952, presenting Assignment 4 for COIT20270: App Development for Mobile Platforms at Central Queensland University. 
  > 
  > Today, I am proud to present the final production release of ElegantLink, a client governance mobile platform engineered for Australian software development consultancy Elegant Media. Over the next ten minutes, I will demonstrate how our system operationalises our Assignment 3 empirical usability findings into a production-grade application featuring direct manipulation gestures, slowed Material 3 container transforms, an asynchronous simulated backend server with session persistence, canonical responsive layouts, and a comprehensive code walkthrough."

---

### [0:35 – 1:10] Slide 2: Persona: Founder Fred (Fred R.)
* **Visual on Screen:** Slide 2 (Founder Fred Profile, Technostress & Outdoor Contrast Needs)
* **Spoken Dialogue:**
  > "Every feature in ElegantLink is calibrated around our empirical persona, Founder Fred—standardised throughout our codebase as Fred R. Fred is a 42-year-old managing director of a retail business in Melbourne who commissioned custom software. He checks his phone in brief 10 to 60-second micro-sessions between warehouse floor inspections and supplier meetings.
  > 
  > Wang and Yu (2024, page 3) demonstrated that technostress directly damages user continuance intention; exposing non-technical founders to Jira backlogs and git churn creates severe friction. Furthermore, Punsongserm and Suvakunta (2025, page 21) showed that mobile legibility collapses under Australian sunlight without high contrast. ElegantLink enforces WCAG 2.1 AA contrast, large 48dp touch targets, and plain-language progress summaries."

---

### [1:10 – 1:40] Slide 3: UCD Framework & Methodology
* **Visual on Screen:** Slide 3 (UCD Framework Diagram `image1.png` & Traceability Matrix)
* **Spoken Dialogue:**
  > "Slide 3 illustrates our User-Centred Design lifecycle across all four assessments. In Assignment 1, we formulated our governance requirements and five usability goals. In Assignment 2, we created the high-fidelity Material 3 prototype. In Assignment 3, we subjected that prototype to empirical testing with three diverse participants. 
  > 
  > Today, in Assignment 4, we close the loop by engineering the three actionable recommendations identified during user testing: slowed container transforms for spatial orientation, direct touch gestures for rapid interaction, and an asynchronous simulated backend server for true state persistence."

---

```
================================================================================
PART 2: BEHAVIORAL SPECIFICATION & USABILITY SYNTHESIS (1:40 – 3:00)
================================================================================
```

### [1:40 – 2:20] Slides 4, 5 & 6: UML Activity Diagrams 1, 2 & 3
* **Visual on Screen:** Slide 4 (AD1 `image2.png`) $\rightarrow$ Slide 5 (AD2 `image3.png`) $\rightarrow$ Slide 6 (AD3 `image4.png`)
* **Spoken Dialogue:**
  > "Slides 4, 5, and 6 show our three UML Activity Diagrams that govern our core user flows. 
  > 
  > Activity Diagram 1 models ambient project status monitoring, where automated background authentication surfaces a traffic-light badge for 10-second glanceability. 
  > 
  > Activity Diagram 2 models deliverable review and contextual feedback, anchoring stakeholder discussions directly beneath design mockups to eliminate fragmented emails. 
  > 
  > Activity Diagram 3 models commercial milestone sign-offs. Because approving milestones triggers binding financial liabilities—specifically \$12,500 AUD—our workflow enforces a neutral two-step confirmation process that completely prevents accidental touchscreen slips."

---

### [2:20 – 3:00] Slides 7 & 8: Privacy Architecture & Usability Evaluation Synthesis
* **Visual on Screen:** Slide 7 (DFD `image5.png` & APPs) $\rightarrow$ Slide 8 (Assignment 3 Empirical Results Matrix)
* **Spoken Dialogue:**
  > "Slide 7 details our privacy architecture. In accordance with LaMonica et al. (2021, page 5), we protect user autonomy through in-app privacy sheets with unbundled opt-in toggles. Dahiya et al. (2024, page 3) emphasised defense-in-depth security; all client data is encrypted with AES-256 and hosted in Australian sovereign facilities in Sydney and Melbourne.
  > 
  > Slide 8 synthesises our Assignment 3 empirical usability testing. Across all three participants, status recognition averaged 8.7 seconds, feedback submission took 38.3 seconds, and error prevention achieved a perfect zero-slip record. The qualitative user feedback directly drove our Assignment 4 upgrades: slowed container transforms, touch gestures, and persistent backend state."

---

```
================================================================================
PART 3: LIVE DEMO 1 — ADAPTIVE & RESPONSIVE LAYOUT (3:00 – 4:45) [0 SLIDES]
================================================================================
```

### [3:00 – 4:45] LIVE DEMONSTRATION: Responsive Screen Layout (<640dp vs >=640dp)
* **Visual on Screen:** **[SWITCH FULL SCREEN TO DARTPAD.DEV RUNNING APP]**
* **Presenter Action:**
  1. Show mobile view ($<640\text{dp}$). Point mouse to bottom `NavigationBar`.
  2. Slowly drag preview window handle wider past $640\text{dp}$.
  3. Show the dynamic transition to left `NavigationRail` and 2-column card reflow.
  4. Drag window back to mobile width to show seamless reversible adaptation.
* **Spoken Dialogue:**
  > "Now, let's transition to our first live demonstration on DartPad: our canonical responsive and adaptive screen layout.
  > 
  > In this mobile viewport under 640dp **[Point mouse to mobile preview]**, ElegantLink utilizes a canonical Material 3 bottom NavigationBar. Notice the filled active indicator pills, bolded active labels, and unbolded unselected states. This layout places all primary destinations directly within Fred's natural thumb zone for comfortable one-handed operation while walking warehouse floors.
  > 
  > Now, watch closely as I expand the viewport width wider, simulating Fred opening the app on his iPad or a desktop web browser **[Slowly drag browser width handle past 640dp]**.
  > 
  > The navigation dynamically transforms: the bottom bar disappears and an adaptive left NavigationRail docks permanently on the left side of the screen. Simultaneously, using Flutter's LayoutBuilder, our surface content reflows from a single column into an expansive, airy two-column grid. The ambient health card and action card sit side-by-side, maximizing horizontal screen real estate without visual clutter. There are no layout overflow errors or unbounded constraints. It adapts seamlessly across all viewports."

---

```
================================================================================
PART 4: LIVE DEMO 2 — GESTURES & SLOWED TRANSITIONS (4:45 – 6:45) [0 SLIDES]
================================================================================
```

### [4:45 – 5:30] LIVE DEMONSTRATION: Gestures — Swipe-to-Dismiss on Notifications
* **Visual on Screen:** **[DARTPAD APP PREVIEW — NOTIFICATIONS SCREEN]**
* **Presenter Action:**
  1. Tap the Notifications icon in the AppBar.
  2. Perform swipe right on the top notification (revealing green 'Acknowledge' drawer).
  3. Release to dismiss; show the floating SnackBar.
  4. Click the 'UNDO' button on the SnackBar to show reversible restoration!
  5. Perform swipe left on a notification (revealing red 'Archive' drawer).
* **Spoken Dialogue:**
  > "Now, let's demonstrate our direct manipulation gestures, fulfilling a core requirement of Assignment 4.
  > 
  > First, in our Notifications screen **[Open Notifications]**, every alert is wrapped in an interactive Dismissible widget. 
  > 
  > Watch as I swipe this milestone alert to the right **[Swipe right]**: a green drawer emerges with a checkmark icon to acknowledge the notification. When released, the item dismisses and an interactive SnackBar appears with a blue 'UNDO' button **[Tap UNDO]**. Tapping UNDO instantly restores the alert back to the feed.
  > 
  > If I swipe to the left **[Swipe left]**, a red archive drawer appears. This gives Fred tactile, reversible control over his alert stream without tedious menu navigation."

---

### [5:30 – 6:15] LIVE DEMONSTRATION: Slowed Container Transforms & Double-Tap Zoom
* **Visual on Screen:** **[DARTPAD APP PREVIEW — DELIVERABLES & MOCKUP VIEWER]**
* **Presenter Action:**
  1. Navigate to Projects $\rightarrow$ Deliverables.
  2. Tap 'Checkout Screen v3.2' card. Notice the smooth 450ms container expansion!
  3. On the Mockup Viewer canvas, double-tap to zoom in (showing 1.75x magnification and badge).
  4. Double-tap again to reset back to 1.0x.
* **Spoken Dialogue:**
  > "Next, let's examine our slowed transitions and double-tap gesture.
  > 
  > In accordance with the rubric requirement for 'transitions slowed for visibility', all screen pushes utilize our custom ElegantPageRoute set to a deliberate 450-millisecond duration. 
  > 
  > Watch as I tap on this deliverable card **[Tap Checkout Screen card]**: instead of a primitive, jarring screen push, the card physically expands outward using a Material 3 Container Transform with continuous cubic easing.
  > 
  > Now, inside the Mockup Viewer, Fred needs to inspect fine typography details. I double-tap directly on the design canvas **[Double-tap canvas]**. 
  > 
  > Notice the smooth animated zoom to 1.75x magnification, accompanied by an updated status chip reading '1.75x Zoom (Double-Tap to Reset)'. Double-tapping again smoothly restores the canvas back to 1.0x scale. This provides intuitive touch inspection without complex pinch controls."

---

### [6:15 – 6:45] LIVE DEMONSTRATION: Long-Press Cryptographic Inspection
* **Visual on Screen:** **[DARTPAD APP PREVIEW — GOVERNANCE & CERTIFICATE SCREEN]**
* **Presenter Action:**
  1. Navigate to Governance tab.
  2. Tap 'Approve Milestone' $\rightarrow$ Confirm Approval in the two-step dialog.
  3. On the Digital Certificate screen, press and hold (long-press) the Audit Hash row.
  4. Show the modal bottom sheet displaying cryptographic SHA-256 verification and copy button.
* **Spoken Dialogue:**
  > "Our third gesture is long-press cryptographic inspection. 
  > 
  > In our Governance screen, when Fred approves Milestone 2 through our two-step confirmation dialog **[Confirm Approval]**, our simulated backend seals the milestone and generates an immutable digital certificate.
  > 
  > When I press and hold down on the Audit Hash row **[Long-press Audit Hash]**, an accessible modal bottom sheet slides up, displaying the full SHA-256 cryptographic digest, the signer identity, sovereign cloud data guarantees, and a one-tap button to copy the hash for company accounting records."

---

```
================================================================================
PART 5: CODE-LEVEL ARCHITECTURAL EXPLANATION (6:45 – 8:45) [0 SLIDES]
================================================================================
```

### [6:45 – 7:30] CODE WALKTHROUGH: Simulated Backend Server & State Persistence
* **Visual on Screen:** **[SWITCH TO DARTPAD CODE EDITOR / VS CODE]**
* **Presenter Action:** Scroll to lines 260–435 showing `class SimulatedBackendServer` and `class AppStateModel`.
* **Spoken Dialogue:**
  > "Now, let's examine our software architecture at the code level.
  > 
  > Complying with Criterion 1, we eliminated all prototype mock hardcoding. Here at line 264, you can see our SimulatedBackendServer singleton class. It manages persistent in-memory collections for notifications, comments, milestones, and privacy settings. 
  > 
  > Notice that every method—such as fetchNotifications, postComment, approveMilestone, and dismissNotification—is asynchronous. We inject simulated network latency using Future.delayed for 250 to 400 milliseconds. 
  > 
  > In AppStateModel, our ChangeNotifier holds a reference to this backend service. When Fred performs an action, the UI updates optimistically while persisting changes to the backend in real time."

---

### [7:30 – 8:15] CODE WALKTHROUGH: ElegantPageRoute & Gesture Implementation
* **Visual on Screen:** **[DARTPAD CODE EDITOR]**
* **Presenter Action:** Scroll to lines 439–515 showing `class ElegantPageRoute`, and lines 3360–3420 showing `Dismissible`.
* **Spoken Dialogue:**
  > "Looking at line 439, here is our custom ElegantPageRoute class. 
  > 
  > To satisfy the rubric requirement for 'transitions slowed for visibility', both containerTransform and sharedAxis are configured with a deliberate 450-millisecond duration using Curves.easeInOutCubic. It scales content from 90% to 100% while fading between surfaces, completely eliminating primitive Navigator.push pushes.
  > 
  > Further down in NotificationsScreen at line 3362, each card is wrapped in a Dismissible widget with Key(item.id). It implements directional background containers—green for acknowledge and red for archive. On dismissal, it calls state.dismissNotification and dispatches our floating SnackBar with an interactive SnackBarAction for undo restoration."

---

### [8:15 – 8:45] CODE WALKTHROUGH: Responsive Shell & Design Comments
* **Visual on Screen:** **[DARTPAD CODE EDITOR]**
* **Presenter Action:** Scroll to `MainPortalShell` showing `LayoutBuilder` breakpoint at `constraints.maxWidth < 640`.
* **Spoken Dialogue:**
  > "Finally, here in MainPortalShell, our responsive layout is orchestrated using Flutter's LayoutBuilder. We evaluate incoming constraints against our canonical 640dp breakpoint. Under 640dp, the widget tree returns a Scaffold with a bottom NavigationBar; at or above 640dp, it renders a Row containing an adaptive NavigationRail docked on the left.
  > 
  > Throughout the 3,633 lines of code, every major component is documented with design-level docstring comments explaining widget selection, touch target compliance, and persona alignment rather than trivial syntax."

---

```
================================================================================
PART 6: DEPLOYMENT, ACADEMIC INTEGRITY & CONCLUSION (8:45 – 10:00)
================================================================================
```

### [8:45 – 9:20] Slide 16: Progressive Web App (PWA) Deployment
* **Visual on Screen:** Slide 16 (PWA Architecture, GitHub Pages & Web App Manifest)
* **Presenter Action:** Return to presentation slides; briefly show PWA deployment card.
* **Spoken Dialogue:**
  > "Slide 16 details our Progressive Web App deployment. We engineered a complete web manifest and optimized HTML shell, deploying the application via GitHub Pages. 
  > 
  > Clients like Founder Fred can open the hosted URL on their smartphone or tablet and add ElegantLink directly to their home screen. It launches in full standalone mode with native-feel performance, smooth animations, and zero app store installation friction."

---

### [9:20 – 9:45] Slides 17 & 18: Code Architecture & Generative AI Statement
* **Visual on Screen:** Slide 17 (Architecture Summary) $\rightarrow$ Slide 18 (AI Statement & Citations)
* **Spoken Dialogue:**
  > "Slide 17 summarises our six-tier software architecture and single-file DartPad execution. Slide 18 discloses our use of Generative AI as an assistive peer-review tool, with all code logic, gestures, and architectural models personally authored, verified, and debugged by myself. 
  > 
  > Every design decision is grounded in nine peer-reviewed journal articles from the CQU Library, complete with exact citations and page numbers embedded in our slide notes."

---

### [9:45 – 10:00] Slide 19: Submission Links & Conclusion
* **Visual on Screen:** Slide 19 (Universal Deliverables Links & Closing Banner)
* **Presenter Action:** Conclude warmly; point to on-screen links.
* **Spoken Dialogue:**
  > "In conclusion, ElegantLink demonstrates a complete, production-grade mobile application that brings clarity, speed, and peace of mind to commercial software clients. 
  > 
  > All deliverable links—our live DartPad code, deployed PWA on GitHub Pages, private GitHub repository, and video presentation link—are displayed on Slide 19. Thank you for your time, feedback, and guidance throughout COIT20270."

---

## Quick-Glance Cue Cards for Presentation Recording

| Timestamp | Mode / Screen State | Primary Action & Spoken Cue |
| :---: | :--- | :--- |
| **0:00** | Slide 1 (Title) | State name, ID (12284952), unit (COIT20270), and app concept (ElegantLink). |
| **0:35** | Slide 2 (Persona) | Introduce Founder Fred (Fred R.), technostress (Wang & Yu), sunlight glare (Punsongserm). |
| **1:10** | Slide 3 (UCD) | Explain progression from Assignment 1 to Assignment 4 production app. |
| **1:40** | Slides 4–6 (Diagrams) | Walk through Activity Diagrams 1, 2, and 3 (Ambient status, feedback thread, two-step sign-off). |
| **2:20** | Slides 7–8 (Privacy/Data) | Explain APPs/CASFUD sovereign hosting, and Assignment 3 empirical test synthesis. |
| **3:00** | **DartPad App Preview** | **LIVE RESPONSIVE DEMO:** Start at mobile ($<640\text{dp}$); slowly drag window wider past $640\text{dp}$ to demonstrate left `NavigationRail` and 2-column card reflow! *(0 slides)* |
| **4:45** | **DartPad App Preview** | **LIVE GESTURE 1:** In Notifications, swipe right to acknowledge (green), tap UNDO on SnackBar; swipe left to archive (red). *(0 slides)* |
| **5:30** | **DartPad App Preview** | **LIVE GESTURE 2 & MOTION:** Open Mockup Viewer via slowed Container Transform (450ms); double-tap mockup canvas to toggle 1.75x zoom. *(0 slides)* |
| **6:15** | **DartPad App Preview** | **LIVE GESTURE 3:** Approve milestone $\rightarrow$ on digital certificate, long-press Audit Hash to open cryptographic verification modal bottom sheet. *(0 slides)* |
| **6:45** | **DartPad Code Editor** | **CODE WALKTHROUGH 1:** Show `SimulatedBackendServer` (lines 264–435) with async latency (`Future.delayed`) and session persistence. *(0 slides)* |
| **7:30** | **DartPad Code Editor** | **CODE WALKTHROUGH 2:** Show `ElegantPageRoute` (lines 439–515) slowed to 450ms, and `Dismissible` with SnackBarAction UNDO. *(0 slides)* |
| **8:15** | **DartPad Code Editor** | **CODE WALKTHROUGH 3:** Show `LayoutBuilder` breakpoint in `MainPortalShell` and deep design-level docstring comments. *(0 slides)* |
| **8:45** | Slide 16 (PWA) | Explain PWA deployment on GitHub Pages (`manifest.json` and standalone installation). |
| **9:20** | Slides 17–18 (Integrity) | AI collaboration statement, critical student ownership, and 9 CQU library citations. |
| **9:45** | Slide 19 (Conclusion) | Display deliverable links (DartPad, PWA, GitHub, Video) and provide concluding thank you. |
