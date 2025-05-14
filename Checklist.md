# Accessibility Test Checklist – W3C WAI

| Test Area              | Scenario                                                             | Expected Result                                             | Tool/Method            | Result | Notes |
|------------------------|----------------------------------------------------------------------|-------------------------------------------------------------|------------------------|--------|-------|
| Keyboard Navigation    | Navigate all menu items using Tab/Shift+Tab                         | Focus is visible and logical                               | Manual                 |    PASS  |  Focus rigns appear. Logical order. Screenshot added     |
| Skip to Content Link   | Check for skip link                                                  | Link exists and jumps to content                           | Keyboard / Manual      |        |       |
| Screen Reader Labels   | Headings are read in correct order                                  | Logical H1 → H2 structure                                  | NVDA / VoiceOver       |        |       |
| ARIA Landmarks         | Page regions are announced properly                                 | Main, Navigation, Banner announced                         | NVDA / HTML inspection |        |       |
| Color Contrast         | Text vs background color contrast                                   | Meets 4.5:1 (normal), 3:1 (large)                          | Axe / CCA              |        |       |
| Image Alt Text         | Images have accurate `alt` tags                                     | Descriptive alt text or `alt=""` for decoratives           | Axe / Manual           |        |       |
| Zoom / Resize          | Zoom to 200%                                                        | Page remains usable and readable                           | Browser Zoom           |        |       |
| Forms (if applicable)  | Form labels and error handling                                       | Labels readable and errors announced                       | NVDA / Keyboard        |        |       |
| Automated Audit        | Run Axe and Lighthouse                                               | No critical issues, score ≥90                             | Axe / Lighthouse       |        |       |
