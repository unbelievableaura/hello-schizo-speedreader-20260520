# ReadQuick Reference Audit

Reference: https://appsinlaw.com/readquick-speed-reading-on-the-iphone/

The useful design point is not "lots of text moving fast." It is RSVP speed reading: one word at a time, fixed in the same screen position, at a chosen WPM.

Initial application:

- The reader shows only one active word in the center.
- The page is 100vh and completely white.
- Typography is Times New Roman.
- Decoration is intentionally minimal and low-contrast.
- The full copypasta is still loaded and played from `HELLO?` through `Disgusting.`
- Controls are limited to play/pause, speed, reset, and progress.

Current adjustment:

- The page is now less training-tool and more white schizo dispatch.
- The center text still changes through the copypasta, but the main word no longer twitches, flashes, or uses color animation.
- The timing control is a dispatch interval, not a WPM training control.

Latest adjustment:

- The visible header no longer contains reader controls.
- Header content is `HELLO?` as a Times New Roman logo plus `Pump.fun`, `Dexscreener`, and `Community`.
- The previous 1-3 word sentence-tone dispatch was replaced by the stricter hold-to-read pass below.

Hold-to-read adjustment:

- The center reader is back to strict RSVP behavior: exactly one word per stop.
- The previous pass used a held `CLICK HERE` button; that control was replaced by autoplay in the next pass.
- The cadence is 230 WPM, a normal average silent-reading pace instead of a hyper-fast meme cadence.
- The active word is centered and forced onto one line; long words shrink to fit the viewport.
- The filled white-page direction uses ASCII heads and low-contrast copy fragments inspired by the supplied reference image instead of a bitmap dependency.

Autoplay mess adjustment:

- The `CLICK HERE` button was removed.
- The one-word RSVP reader now autoplays at 230 WPM.
- Background box styling was removed from the note scraps, and additional uneven low-contrast copy fragments fill the 100vh white page.
- Pointer movement now emits tiny copypasta text fragments from the cursor and fades them out.
