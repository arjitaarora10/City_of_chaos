# Build a Playable GTA-Style Open-World Game — “CITY OF CHAOS”

Create a realistic, fully playable 3D open-world action game inspired by the freedom and gameplay systems of Grand Theft Auto. Use Three.js with JavaScript or TypeScript, or another suitable browser-based 3D engine.

The game must be interactive, not just a rendered scene, animation, or static demo.

## 1. OPEN-WORLD CITY

Build a large, explorable modern American-style city with:
- Downtown skyscrapers, residential neighborhoods, highways, beaches, bridges, industrial zones, and shops.
- Roads with lane markings, traffic lights, intersections, sidewalks, and parking areas.
- Moving cars, motorcycles, buses, and pedestrians.
- Buildings with collision boundaries and accessible interiors for selected locations.
- A realistic sunset, nighttime lighting, streetlights, weather, rain, and wet-road reflections.
- Ambient city sounds, vehicle engines, horns, footsteps, and sirens.

The world should feel alive. Pedestrians should walk along sidewalks, traffic should obey basic road rules, and vehicles should avoid obvious collisions.

## 2. THIRD-PERSON PLAYER

Create a visible, animated human character with a smooth third-person camera.

**Controls:**
- W/A/S/D — Walk and run.
- Mouse — Rotate camera.
- Shift — Sprint.
- Space — Jump.
- C — Crouch.
- E — Enter or exit vehicles and interact with objects.
- F — Melee attack.
- Left mouse button — Fire an equipped weapon.
- R — Reload.
- M — Open the city map.
- Tab — Open character and inventory menu.
- Esc — Pause.

Movement must work immediately. Implement camera-relative movement, acceleration, gravity, jumping, collision detection, and smooth character animations.

Never allow the character to become invisible, freeze in place, fall through the road, or get trapped inside buildings.

## 3. DRIVING SYSTEM

Driving is a core feature, not an optional extra.

- Allow the player to approach a parked or moving vehicle and press E to enter.
- Animate the character entering and exiting the vehicle.
- Switch smoothly from the walking camera to the driving camera.
- W accelerates, S brakes or reverses, A and D steer, and Space activates the handbrake.
- Implement vehicle acceleration, braking, steering, friction, suspension effects, and collisions.
- Add different vehicle classes: sports cars, sedans, SUVs, motorcycles, and trucks.
- Give vehicles different handling, top speeds, and acceleration.
- Allow the player to steal or borrow vehicles within the game's fictional world.
- Add vehicle damage, tire skids, engine audio, and visible brake lights.
- Ensure the player can reliably exit any vehicle and resume walking.

## 4. POLICE AND WANTED SYSTEM

Create a working five-level wanted system.

- Criminal actions witnessed by police increase the wanted level.
- Police vehicles pursue the player when wanted.
- Police officers can exit vehicles and chase the player on foot.
- Higher wanted levels trigger additional police units and roadblocks.
- The player can attempt to escape by breaking line of sight and leaving the search area.
- A search indicator should show when police are still looking for the player.
- Wanted stars decrease when the player successfully evades pursuit.

Police AI must react to the player's actual position and vehicle, not move randomly.

## 5. MISSIONS AND STORY

Create a fictional story about a street racer who becomes involved in a citywide criminal conspiracy.

Include these playable missions:

**Mission 1 — First Ride:** Find a car and drive to a marked destination.

**Mission 2 — The Delivery:** Drive through the city while avoiding police attention.

**Mission 3 — Street Race:** Race AI-controlled opponents through checkpoints.

**Mission 4 — Getaway:** Escape a police pursuit using driving skills.

**Mission 5 — The Warehouse:** Infiltrate a guarded location and retrieve a fictional data drive.

**Mission 6 — Final Escape:** Complete a multi-stage mission involving driving, exploration, and a final chase.

Each mission must have objectives, checkpoints, success and failure conditions, and rewards. Include a mission marker in the world and on the map.

## 6. WEAPONS AND COMBAT

- Include fictional or generic weapons with ammunition and reloading.
- Add melee combat, aiming, hit detection, and enemy health.
- Create enemy NPCs with patrol, alert, chase, and attack behaviors.
- Add basic cover and line-of-sight detection.
- Implement damage feedback, character defeat, and respawning.
- Keep combat separate from vehicle controls so the two systems do not conflict.

## 7. ECONOMY AND CHARACTER PROGRESSION

- Give the player starting cash.
- Reward mission completion with money.
- Add garages where vehicles can be stored.
- Include vehicle purchasing and customization.
- Add clothing shops, convenience stores, and safehouses.
- Save the player's cash, unlocked vehicles, and completed missions using local browser storage.

## 8. GTA-STYLE HUD

Create a polished game interface featuring:
- A circular minimap with roads, the player's direction, mission markers, and police indicators.
- Health and armor bars.
- Cash balance.
- Wanted stars.
- Current weapon and ammunition.
- Vehicle speedometer while driving.
- Mission objectives and waypoint distance.
- In-game phone with fictional contacts and mission notifications.
- Pause menu with resume, settings, and restart options.

The UI must update dynamically from actual game state.

## 9. TECHNICAL ARCHITECTURE

Build the game in a stable, modular way.

Suggested systems:
- Game initialization and rendering.
- Player controller.
- Third-person camera controller.
- Vehicle physics and vehicle switching.
- City and road generation.
- Pedestrian and traffic AI.
- Police and wanted-level manager.
- Combat and health system.
- Mission manager.
- HUD and minimap.
- Save/load system.

Use delta-time-based updates, optimized geometry, instancing for repeated objects, and distance-based updates for distant NPCs.

Use reliable collision detection and a consistent coordinate system. Make all essential assets load correctly. If external assets are unavailable, create simplified procedural 3D models rather than leaving the world empty.

## 10. REQUIRED DEVELOPMENT ORDER

Build the game incrementally in this exact order:

1. Create a 3D ground plane, city blocks, and visible player.
2. Implement and test player movement and the third-person camera.
3. Add one fully drivable vehicle and working enter/exit mechanics.
4. Add roads, buildings, and basic traffic.
5. Add the minimap and waypoint navigation.
6. Add police pursuit and the wanted system.
7. Add one complete playable mission.
8. Expand the city, missions, combat, and progression.
9. Improve graphics, audio, animations, and environmental details.

## 11. TESTING REQUIREMENTS

Before finishing, verify that:
- W/A/S/D move the character correctly.
- The camera rotates smoothly and follows the player.
- The player can enter a car, drive it, stop, exit, and walk again.
- Vehicles collide with buildings and other vehicles.
- Traffic and pedestrians move.
- Mission markers update correctly.
- Police chase the player when wanted.
- The player can lose the police.
- Missions can be completed and failed.
- Restarting does not leave broken game state.
- The game runs in the browser without critical console errors.

**IMPORTANT:** Prioritize actual gameplay over visual complexity. Do not generate a beautiful city with broken controls. Do not create fake buttons or claim that unfinished features work. If the complete game is too large for one generation, deliver a fully working first version with movement, driving, a small city, a minimap, and one mission before expanding it.

Start by implementing the playable game, then test each system before adding the next one.
