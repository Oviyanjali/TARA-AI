# TARA Mission Simulator

TARA (Tactical Autonomous Response Assistant) turns a spoken command into a checked drone mission plan.

> "Hey Tara, search the flooded area." → TARA plans it → the Safety Guard checks it → you say "yes" to fly.

**The AI proposes. Fixed code decides. A person approves.**

## How to run
1. Download `tara-simulator-offline.html` from this repository.
2. Open it in **Google Chrome**. No install or internet needed.
3. Pick a mission and click **Launch TARA with voice**, then allow the microphone.
4. Say **"Hey Tara, patrol the fence in sector Bravo"**, then **"yes"**.

Typed commands work too. Voice works best in Chrome on a laptop.

## What's inside
- **Voice control:** "Hey Tara" wake word, English, Hindi and Tamil commands
- **Safety Guard:** 14 checks on every plan (geofence, no-fly zones, altitude, terrain, people, range, battery, wind, GNSS, link, temperature and more), plus a 10 Hz monitor that can hold, return home or land on its own
- **Fault injection:** GNSS jamming and spoofing, link loss, wind, overheating, battery cell failure
- **Sensors:** day, night-vision and thermal camera views, radar, tactical map, live tracks
- **Missions:** border watch, night intrusion, warehouse security, flood rescue, jamming stress test
- **Reports:** contact alerts, location sharing, SALUTE and after-action reports

## Try this
- "Hey Tara, search the flooded area", then "yes"
- "Climb to 300 metres": the Guard blocks it (above the 120 m ceiling)
- "Fly across the border": the Guard blocks it (geofence)
- Use the fault buttons to jam GNSS and watch the Guard respond

## Test results (in simulation)
| Check | Result |
|---|---|
| Unsafe or broken flight plans approved | 0 of 21,920 |
| Simulated flights with random faults | 500 flights, 0 drones lost |
| Mission scenario runs | 140 of 140 passed, 0 false alerts |

## Note
This is a software simulation. Nothing here is flight data, and it has not flown a real aircraft. Detection ranges are modelled, and the building scan is a labelled concept.

Built as a team project.
