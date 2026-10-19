# Resetting progress

Progress is stored in the browser on the device (local storage for this site).
There is no server copy, so a reset always runs on the device itself: open one
of the links below on the device, and the app applies the reset, saves, and
shows a confirmation message.

App: https://kriskrss.github.io/workout-coach/
Reset page (buttons for all of the links below): https://kriskrss.github.io/workout-coach/reset.html

## Reset links

| Link | Effect |
| --- | --- |
| `?reset=today` | Clear every tick for today's plan |
| `?reset=today-lesson` | Clear today's lesson only (episode ticks + Lesson done) |
| `?reset=day:YYYY-MM-DD` | Clear all ticks for one calendar day, e.g. `?reset=day:2026-10-18` |
| `?reset=day:YYYY-MM-DD:lesson` | Clear one day's lesson only |
| `?reset=day:YYYY-MM-DD:strength` | Clear one day's strength ticks only |
| `?reset=day:YYYY-MM-DD:cardio` | Clear one day's cardio ticks only |
| `?reset=week` | Clear all ticks in the current 7-day window |
| `?reset=all` | Clear all progress (ticks, phase progress, catch-up state). Playback speed and coach on/off settings are kept |

Full form example: https://kriskrss.github.io/workout-coach/?reset=today-lesson

Unrecognised values change nothing and say so in the confirmation message.
The same resets are available inside the app, in the collapsed
"Reset progress" panel (each asks for a confirming second tap).
