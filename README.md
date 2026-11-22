# Classroom Timer / Playtime Loss Tracker — Version 3.8

A standalone, GitHub Pages-ready classroom timer. Version 2.0 is not modified.

## Files
- `index.html`: interface and independent visual layers
- `styles.css`: responsive classroom and controls
- `app.js`: countdown, students, voices, teacher selection, clock, tests
- `assets/classroom.jpg`: illustrated classroom (static artwork)
- `assets/teacher-*.png`: six selectable teacher overlays (Dave, Ms. Grizzle, Turbo Fox, Principal Rex, Mr. Blocks, Professor Gizmo)

## GitHub Pages
Create a **new repository** (do not overwrite the working Version 2.0 repository). Upload the entire contents of this folder, keeping relative paths. Under **Settings → Pages**, choose **Deploy from a branch**, branch **main**, folder **/(root)**. Visit the GitHub Pages URL when deployed.

## Testing
1. Confirm **APP READY** appears at bottom left of the scene. This confirms JavaScript ran.
2. Verify the analog clock moves and shows the local device time.
3. Use TEST → 10-SECOND TEST and TEST RELEASE ANNOUNCEMENT.
4. Add two names; click + for one student; START. The student with one mark releases after two minutes, the other after four.
5. In NAMES / VOICE / TEACHER, switch among the six teachers. Teacher is hidden in general timer mode by default; select Both timer modes to show them in both.
6. Use FULL SCREEN on the school Newline board. On a mobile device, audio availability depends on its browser and voice support.

## Notes
- No external libraries, fonts, or network services are used.
- The Newline's screen and clock are overlaid with functioning HTML/SVG. The classroom background is not interactive.
- The artwork includes static board labeling and an illustrated clock beneath the working overlays; the working elements are drawn on top.
- Teacher PNGs are independent of the background. Amy's cutout was extracted from an image with a checkerboard background; check edges on a large display.
- The application is not yet verified on a physical Newline board; this is a test build.

## Version 3.1 updates
- Approved 20-dot classroom background (4 rows of 5, muted and smaller).
- Teacher cutouts scaled taller and placed left of the Newline; teacher visibility configurable.
- Wall clock aligned over the illustrated clock and updated live.
- Nonmodal draggable settings window.
- Activity dropdown: Playtime, Free Choice, or custom text.
- All assets remain local; no external dependencies.

## Version 3.2 layout adjustments
- Teacher layer enlarged and moved left, with feet kept on the carpet.
- Wall clock overlay shifted right and slightly down to cover the illustrated clock.
- Smaller heading and timer footer to show six student names in three rows of two without scrolling at typical desktop/fullscreen sizes.

## Version 3.3 changes
- Background now has no printed wall clock; the working SVG clock is the only clock.
- Teacher layer widened by 40.5% relative to v3.2, with the same floor baseline.
- The timer code and other features remain unchanged.

### v3.4 placement adjustment
Teacher standing layer shifted 2.6 percentage points to the right, with size and feet height unchanged.

### Version 3.5
Amy is scaled approximately 10% shorter than Dave and her PNG has its internal checkerboard gap removed, preserving actual alpha transparency. Teacher feet remain on the same floor anchor.


## Version 3.6: teacher choices
Choose Dave, Amy (placeholder), Ms. Grizzle, Turbo Fox, Principal Rex, Mr. Blocks, or No teacher in Names / Voice / Teacher. Each is a separate transparent PNG in `assets/` with a shared floor baseline and individually adjustable CSS scale. All other timer, clock, activity, voice, and fullscreen behavior is inherited from v3.5. The new character sizes are initial estimates and should be visually tested on the Newline screen.


Version 3.7: Repositioned Grizzle, Turbo Fox, Principal Rex, and Mr. Blocks rightward and moved all teacher cutouts above the monitor layer. Dave and Amy remain unchanged.

## Version 3.8
Replaced Amy with Professor Gizmo, a separate transparent PNG. Existing classroom, timer, clock, and other character positions are unchanged.

## Version 3.9 positioning update

Professor Gizmo, Principal Rex, and Mr. Blocks have been shifted left by approximately 3.7–3.8 percentage points of scene width and lowered 1.8 percentage points to give a slight forward placement without resizing them. Their foreground z-index remains above the Newline monitor. Dave, Ms. Grizzle, and Turbo Fox are unchanged. All timer, clock, activity, voice, and teacher selection logic is unchanged. Verify chair clearance and names on the intended display before publishing.
