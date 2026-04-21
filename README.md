# Lab 02: Interface Design & Safety-Critical Systems
---

### Student Information
* **Name:** Bisma
* **Seat No:** B23110006022 
* **Section:** A

---

## 1. Why do UIs Fail?
User Interfaces fail when they prioritize machine logic or technical efficiency over human cognitive and physical limitations.

### Key Factors:
* **Low Error Tolerance:** Systems fail when a minor "slip" (like an accidental extra keypress) leads to a catastrophic outcome.
* **High Cognitive Load:** Forcing users to process too much unorganized data at once exceeds short-term memory limits.
* **Designing for Machines:** Prioritizing how code functions rather than how a human naturally completes a task leads to unusable designs.
* **Poor Visibility:** Failing to clearly display the system state prevents users from verifying data before execution.

---

## 2. Failure Analysis (Numeric Keypad)
The original interface utilized a numeric keypad for dose entry. In safety-critical environments, this design is dangerous because it lacks constraints.

### Observation:
* **Exponential Errors:** If a user intends to enter **137 mg** but accidentally taps an extra digit, the input becomes **1372 mg**.
* **Lethal Slips:** This single key slip causes a **10x overdose**, which is potentially lethal in medical contexts.
* **Lack of Constraints:** Free-form entry allows for values that far exceed safe operating limits without immediate physical friction.

---

## 3. Redesign Logic
The redesign focuses on **Error-Tolerant Design** to eliminate the risk of accidental overdoses by restricting how data is entered.

### Strategies Applied:
* **Constraint-Based Input:** The keypad is replaced with individual **+** and **−** buttons for each digit.
* **Prevention of Decimal Shifts:** By isolating digits, it is physically impossible for a single accidental click to shift the entire value by a power of ten.
* **Forced Verification:** Adjustment controls are separated from the final dose summary to force a moment of human verification before action.

---

## 4. UI Principles (HCI Standards)
The following Human-Computer Interaction (HCI) principles were applied to the new interface to ensure safety and clarity:

* **Visibility of System State:** The "TOTAL DOSE" is displayed in large, bold typography in a dedicated area so the user always knows the current value.
* **Error Tolerance:** The system is designed to be highly tolerant, making mistakes easy to catch and difficult to commit.
* **Constraints:** By restricting input methods to increment/decrement steps, we guide the user toward safe and intentional behavior.
* **Affordance:** Clear **+** and **−** buttons provide an immediate visual understanding of how to interact with each digit.

---
