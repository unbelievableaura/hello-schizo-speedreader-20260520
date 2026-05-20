# HELLO? Design Plan And Audit

## Plan

- Keep the site pure white and Times New Roman, with `HELLO?` as the literal brand signal.
- Use a strict RSVP reader in the center: one word, fixed position, no animation on the main word.
- Autoplay the reader at 230 WPM without an on-page control button.
- Fill the 100vh page with generated floating stern heads inspired by the supplied reference image, plus uneven exact copypasta fragments around the reader.
- Emit tiny copypasta fragments from the cursor on pointer movement.
- Keep the background copy strict: decorative text must be literal text from the supplied copypasta, not new jokes or paraphrases.

## Audit

- Main reader: one active `.token` is rendered at a time from the copypasta word list.
- Speed: `STEP_DELAY` is calculated from `AVERAGE_WPM = 230`.
- Interaction: autoplay is default; arrow-key stepping remains supported for manual checking.
- Cursor effect: pointer movement creates tiny fading text fragments and removes them after animation.
- Layout: the active word uses `white-space: nowrap` and shrinks if it would exceed the viewport.
- Theme: white background, black/gray Times New Roman, no color-heavy treatment.
- Generated image assets: Imagegen produced a three-head chroma-key sheet, locally keyed into transparent PNGs, then split into three floating assets.
- Risk: floating heads are decorative and intentionally low-contrast; they are hidden from assistive tech through the background field's `aria-hidden`.
