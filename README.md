# Fix and Fly

A retro space mission design game made for the NASA Space Apps Challenge 2026
(challenge: *Space Mission Design Game*).

You are the pilot of a repair mission. Space weather has damaged three real-world-inspired
spacecraft. Design a rocket on a budget, fly out, diagnose each spacecraft, choose the right
repair, survive an unknown solar event, and report your findings to Mission Control.

**Play:** open `index.html` in any modern browser. No install or internet needed
(the pixel font falls back to a system font offline).

## How to play

1. **Mission brief:** read the need, goals, segments and requirements.
2. **Design:** choose a body, engine and interior within a $100M budget. Every part has a
   cost, mass and real trade-off.
3. **Fly:** fly from Earth to the damaged spacecraft (arrow and mini map show the way).
4. **Diagnose:** stay close for 3 seconds to collect telemetry, magnetic-field and radiation
   readings.
5. **Repair:** press Fix and choose the repair that matches the diagnosis. Two wrong
   repairs fail the mission.
6. **Survive the event:** repairing triggers an unknown solar event. Read the clue and buy
   upgrades. Keep your hull above 25%.
7. **Report:** fly into the Earth safe zone (it also restores hull and fuel) to transmit
   the data. Collect stars on the way for extra budget.
8. Finish all three to unlock a harder level.

Controls: arrows or WASD to fly, X to scan/fix, R repairs hull (+8, $6), F refuels ($5).
On-screen buttons work on touch devices.

## How it follows NASA’s mission design process

The structure is based on NASA’s *Design and Develop Science Missions* webinar
(Systems Engineering Series, March 2025): identify need and goals, define the concept,
define requirements, design, build and verify, implement.

| NASA step | In the game |
|---|---|
| Need and goals | Mission brief |
| Segments (launch, space, ground, user) | Rocket, spacecraft, Earth safe zone, findings |
| Requirements | R1 to R4 shown in the brief |
| Design | Body, engine and interior choice under budget |
| Implement | The flight and repair |
| Verify | End report checks each requirement as MET or NOT MET |

The pilot handles four jobs at once: navigation, spacecraft integrity and repair,
data analysis, and communications with Earth.

## Real data and events behind the game

| Game element | Real basis |
|---|---|
| Deep-space radiation rises to 1.84 mSv/day | Curiosity RAD instrument, measured inside the cruise vehicle to Mars |
| Safe zone about 0.7 mSv/day | ISS crews receive roughly 0.4 to 1.0 mSv/day |
| Basic shell does almost nothing against cosmic rays; polyethylene about 15% better, and 50% better against flares | NASA Science archive, plastic shielding article (2005) |
| Sunlight strength rises with 1 / distance² | Inverse-square law of solar flux |
| Earth observer, power failure | Midori-II (ADEOS-II), October 2003 Halloween storms |
| Comms constellation, drag | Starlink loss, February 2022 geomagnetic storm (38 of 49 satellites) |
| Data relay, Earth sensor errors | Kodama relay satellite, October 2003 storms |

Sources consulted: NASA Design and Develop Science Missions webinar PDF; NASA Technical Reports
Server (polyethylene shielding, NTRS 20205002815); NOAA National Weather Service Starlink report;
NASA Goddard SVS Starlink page; JAXA/MEXT Midori-II records; IEEE Spectrum, “Extreme Solar
Storm Strikes Earth”; reporting on the Curiosity RAD results (Science, 2013).

## What is simplified

This is a game, not a simulator.

- The map is not to scale, and the spacecraft do not orbit.
- Costs, masses, thrust, fuel use, event damage and upgrade effects are invented for
  gameplay. Only the proportions (for example, shielding choices and the 1/d² sunlight rule)
  follow real data.
- Body heat limits (2x to 6x Earth sunlight) are estimates.
- In the real events the spacecraft were lost. In the game they can be repaired.
- Mission data is embedded in the game. It does not call live NASA services.

## Use of AI tools

Game concept, mechanics and theme: No Game No Life.

Claude (a large language model by Anthropic) was used to help refine the game design,
research real events and sources, write the game code (HTML, CSS and JavaScript), and draft
in-game educational text. Real-data values were checked against the sources listed above.

No NASA logos, flags or mission identifiers are used.

## Future work

- Team mode with four roles (navigator, engineer, scientist, communications).
- Orbiting spacecraft, inspired by NASA Mission Viz.
- Trajectory planning with NASA GMAT.
- More scenarios from NASA’s DONKI space weather database.
- Art, sound and a tutorial.

## License

[Choose a license, for example MIT, and add a LICENSE file.]
