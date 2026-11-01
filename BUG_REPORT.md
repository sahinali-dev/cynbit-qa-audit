# Bug & Issue Report

### Summary of Findings
| Bug ID | Title | Severity | Priority | Category |
| :--- | :--- | :--- | :--- | :--- |
| **BUG-01** | Typography Clipping on 'Map' Heading | Low | Low | Visual / UI |
| **BUG-02** | Empty Box Containers in System Logic Section | Medium | Medium | UI / Rendering |
| **BUG-03** | Typography Clipping on 'Blueprint' Heading | Low | Low | Visual / UI |
| **BUG-04** | Android Nav Menu Ambiguity ('Blog & Contact') | Low | Medium | UX / Navigation |
| **BUG-05** | 'Write Us' Desktop Click Event Listener Issue | High | High | Functional / Cross-Platform |

---

### Detailed Bug Descriptions

#### BUG-01: Typography Clipping on "Navigation Map"
- **Severity:** Low | **Priority:** Low
- **Component:** Header Section ("Map")
- **Description:** The right edge of the letter 'p' in the word "Map" is clipped off visually.
- **Root Cause:** Container overflow restriction (`overflow: hidden`) or insufficient right-padding on the text bounding box.
- **Steps to Reproduce:**
  1. Navigate to the Navigation Map section on Desktop/Mobile.
  2. Observe the right boundary of the word "Map".
- **Expected Result:** Typography should render completely without glyph truncation.
- **Actual Result:** Letter 'p' appears partially cut off on the right side.

![Bug - 01 Proof](./screenshots/Bug%20-%2001.png)

----

#### BUG-02: Empty Box Elements in "System Logic – Preparation"
- **Severity:** Medium | **Priority:** Medium
- **Component:** System Logic Section
- **Description:** Empty box containers render below section bars without visible text or content.
- **Steps to Reproduce:**
  1. Scroll to the "System Logic – Preparation" section.
  2. Inspect the content containers under the header bar.
- **Expected Result:** Boxes should contain text/data, or display a clean loading/empty state.
- **Actual Result:** Blank placeholder boxes render without content.

![Bug - 02 Proof](./screenshots/Bug%20-%2002.png)

----

#### BUG-03: Typography Clipping on "Contact – Blueprint"
- **Severity:** Low | **Priority:** Low
- **Component:** Contact Section ("Blueprint")
- **Description:** The bottom-left corner of the letter 'p' in "Blueprint" is cut off.
- **Expected Result:** Full visibility of typographic characters.
- **Actual Result:** Character 'p' edge is clipped by container boundaries.

![Bug - 03 Proof](./screenshots/Bug%20-%2003.png)

----

#### BUG-04: Non-Interactive Heading in Android Navigation Menu
- **Severity:** Low | **Priority:** Medium
- **Component:** Android Mobile Navigation Menu
- **Description:** "Blog & Contact" displays in large bold text resembling a clickable navigation link, but tapping produces no action.
- **Expected Result:** Menu items with link styling should navigate to target sections/pages.
- **Actual Result:** Item behaves as a static heading without navigational affordance.


#### BUG-05: Desktop Primary Click Defect on "Write Us" Button
- **Severity:** High | **Priority:** High
- **Component:** Contact Section ("Write Us" CTA)
- **Description:** Clicking "Write Us" on Desktop triggers a hover elevation animation but fails to initiate the mail action on primary click. Right-clicking to open in a new tab reveals `mailto:opportunities@cynbit.in`. Tapping on Android mobile correctly launches the native email composer.
- **Steps to Reproduce:**
  1. Navigate to "Contact" on a desktop browser.
  2. Left-click the "Write Us" button.
- **Expected Result:** Primary left-click opens default desktop email client (or triggers mailto event).
- **Actual Result:** Button elevates on hover, but direct left-click triggers no window action.

![Bug - 05 Proof](./screenshots/Bug%20-%2005.png)

----

---

<!-- ![Write Us Bug Proof](./screenshots/write-us-bug.png) -->
