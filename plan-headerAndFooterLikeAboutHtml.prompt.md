## Plan: Align project.html Header/Footer with about.html

TL;DR: Update `project.html` so its header and footer match the layout and styling already used by `about.html` and `index.html`.

**Steps**
1. Replace the current inline `header` and `footer` sections in `project.html` with the shared site header/footer structure from `about.html`.
   - Use the `top-bar` block and `nav.navbar` markup from `about.html`.
   - Use the `footer` markup from `about.html`.
2. Adjust the nav links in `project.html` so the active page state reflects the Projects page.
   - Keep `Home`, `About`, `Services`, `Projects`, and `Contact` links.
   - Mark the `Projects` link as active.
3. Remove the inline header/footer CSS embedded in `project.html`.
   - The project page should rely on `css/index.css` and existing shared styles.
4. Confirm `project.html` still loads any required fonts, icon styles, and scripts already present in the page head.
5. Test locally by opening `project.html` in a browser and verifying the header/footer visually match `about.html`.

**Verification**
1. Open `project.html` in the browser and verify the top bar and navigation match the look/structure of `about.html`.
2. Verify the footer content and layout match `about.html`.
3. Confirm the `Projects` menu item is visually active.
4. Ensure there are no missing stylesheet or script errors in browser console.

**Decisions**
- Use the shared site layout from `about.html` rather than preserving the current standalone header/footer from `project.html`.
- Keep `project.html` content otherwise unchanged.
