# Improvement Recommendations

## 1. Development Team Fixes (Prioritized)
1. **Fix Primary Event Listener on "Write Us" Button (High Priority):**  
   Ensure the `href="mailto:opportunities@cynbit.in"` is attached directly to the clickable `<a>` wrapper or fix JavaScript `onClick` event delegation so desktop clicks trigger the default mail client properly.
2. **Resolve Layout Overflow & Line Heights (Medium Priority):**  
   Adjust container `padding-right` and CSS `line-height` attributes on header titles ("Map", "Blueprint") to prevent glyph clipping across web fonts.
3. **Data Binding & Empty State Handling (Medium Priority):**  
   Implement visual fallback/empty states for containers in "System Logic" if dynamic content fails to load or is unassigned.
4. **UX Affordance Adjustment on Mobile Nav (Low Priority):**  
   Differentiate non-clickable category headers from actionable links in the mobile menu (e.g., using visual divider lines or distinct typography sizing).
