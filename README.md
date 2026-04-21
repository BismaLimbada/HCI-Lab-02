# Lab 02: Automated Syringe Dose Calculator
Live Deployment: https://bismalimbada.github.io/HCI-Lab-02/
---

### Student Information
* **Name:** Bisma
* **Seat No:** B23110006022 
* **Section:** A

---

## 1. Why do UIs Fail?
User Interfaces fail when they prioritize machine logic or technical efficiency over human cognitive and physical limitations.

### Key Factors:
* **Low Error Tolerance:**  Small mistakes cause major consequences
* **High Cognitive Load:** Too much information overwhelms users
* **Designing for Machines:** Built for machines, not users
* **Poor Visibility:** System state is unclear

---

## 2. Failure Analysis (Numeric Keypad)
The original interface utilized a numeric keypad for dose entry. In safety-critical environments, this design is dangerous because a small mistake (e.g., typing 1372 mg instead of 137 mg) can cause a 10× overdose. This happens due to:
* No input constraints
* High chance of accidental key presses
* Lack of immediate error prevention

---

## 3. Redesign Logic
The redesign focuses on **Error-Tolerant Design** to eliminate the risk of accidental overdoses by restricting how data is entered.

* **Constraint-Based Input:** Replaced keypad with + / − controls for each digit
* **Prevention of Decimal Shifts:** Prevented large value jumps from single mistakes
* **Forced Verification:** Separated controls from final dose display for verification before action

---

## 4. UI Principles (HCI Standards)

* **Visibility of System State:** Dose clearly displayed
* **Error Tolerance:** Mistakes are minimized
* **Constraints:**  Limited, safe input methods
* **Affordance:** Clear + / − interactions


---
