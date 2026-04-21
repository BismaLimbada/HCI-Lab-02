# Lab 02: Automated Syringe Dose Calculator

## Live Deployment: (https://bismalimbada.github.io/HCI-Lab-02/)

### Student Information

* **Name:** Bisma
* **Seat No:** B23110006022
* **Section:** A

---

## 1. Why do UIs Fail?

User Interfaces fail when they focus more on machine logic than human needs and limitations.

### Key Factors:

* **Low Error Tolerance:** Small mistakes cause serious outcomes
* **High Cognitive Load:** Too much information overwhelms users
* **Designing for Machines:** Not user-friendly
* **Poor Visibility:** System status is unclear

---

## 2. Failure Analysis (Numeric Keypad)

The original interface used a numeric keypad for dose entry, which is risky in critical situations. A small error (e.g., 1372 mg instead of 137 mg) can cause a major overdose due to:

* No input limits
* Easy accidental key presses
* No immediate error prevention

---

## 3. Redesign Logic

The redesign applies **Error-Tolerant Design** to reduce overdose risks by controlling how data is entered.

* **Constraint-Based Input:** Used + / − instead of keypad
* **Prevention of Decimal Shifts:** Avoids large value mistakes
* **Forced Verification:** Separate display for checking before action

---

## 4. UI Principles (HCI Standards)

* **Visibility of System State:** Dose is clearly shown
* **Error Tolerance:** Reduces chances of mistakes
* **Constraints:** Safe and limited input methods
* **Affordance:** Clear + / − controls

---

If you want, I can make it **even more concise (like 1-line bullet style)** or help you format it for submission (PDF/Word).
