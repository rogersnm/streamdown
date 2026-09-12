# Streamdown animation regression recordings

Side-by-side headless Chromium recordings of unpatched and patched Streamdown, based on upstream fdf4e331920681d4a6eb22467973f46bdd4b177d. Both panes receive identical text and options in React Strict Mode: 50 ms input updates, a 250 ms fade, and a 10 ms stagger. Scenarios include prose, Markdown lists and formatting, bursts, and replaying a burst.

- [Real-time comparison](comparison.mp4)
- [Same recording at quarter speed](comparison-slow.mp4)

The patch preserves active animations across updates, lets finite animations finish when streaming stops, and clears removed blocks' animation history so replayed opening words animate again. The demo uses illustrative text only. These media assets are kept separately from the upstream source PR.
