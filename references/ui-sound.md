# UI sound

Read for: sounds inside an app interface. Taps, clicks, toggles, confirm and error cues, notifications, typing.

## Rules

- Most interactions should make no sound. Sound only key moments (confirm, error, notification, a rare celebration), never every tap or small motion, and never on hover.
- Keep sounds short: taps and clicks under about 150 ms, confirmations 100–250 ms, notifications under about 500 ms. Trim them shorter than feels right alone, because they repeat all day.
- Let pitch carry the meaning: rising for success, forward and "on"; falling or lower for error, cancel, back and "off"; one flat tone for neutral taps and selection. Success and error must be tellable apart without looking.
- Make frequent sounds higher, brighter and quieter, with no melody or personality. Save lower, fuller sounds for rare moments.
- Build every sound as one family: same timbre, only pitch and length change, all at the same perceived loudness.
- Cut each file to start on its first transient. Leading silence makes the interface feel laggy.
- For sounds that repeat fast (typing, ticks), ship a few variants and never play the same one twice in a row.

## Tool

`earshot` (Python; needs ffmpeg and about 1.1 GB of models). Built for sound on code-made films, but it can render UI sounds offline (`earshot sfx render ui_pop/soft -o pop.wav`) and check them for clicks, clipping and cut tails (`earshot sfx check pop.wav`). Source: https://github.com/Leonxlnx/earshot (MIT).

Before shipping its sounds in an app: it ships no audio files, only code that renders each sound to a WAV by id (e.g. `earshot sfx render toggle/on -o toggle-on.wav`). The code is MIT, but nothing states the terms for the rendered WAVs, so check with the author for a paid app. It is built for film soundtracks, so listen on a phone speaker first.
