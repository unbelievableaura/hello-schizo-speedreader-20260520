# HELLO? Design Plan And Audit

## Plan

- Keep the site pure white and Times New Roman, with `HELLO?` as the literal brand signal.
- Use a strict RSVP reader in the center: one word, fixed position, no animation on the main word.
- Make progress intentional: `CLICK HERE` advances only while held, at 230 WPM.
- Fill the 100vh page with low-contrast ASCII: floating stern heads inspired by the supplied reference image, plus copypasta fragments around the reader.
- Keep bitmap generation optional for a later pass. The current shipped version uses code-native ASCII so it is lightweight, deterministic, and deploy-safe.

## Audit

- Main reader: one active `.token` is rendered at a time from the copypasta word list.
- Speed: `STEP_DELAY` is calculated from `AVERAGE_WPM = 230`.
- Interaction: pointer hold, touch hold, Space/Enter hold, and arrow-key stepping are supported.
- Layout: the active word uses `white-space: nowrap` and shrinks if it would exceed the viewport.
- Theme: white background, black/gray Times New Roman, no color-heavy treatment.
- Risk: ASCII heads are decorative and intentionally low-contrast; they are hidden from assistive tech with `aria-hidden`.
