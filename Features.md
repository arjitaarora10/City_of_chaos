Here is the complete breakdown of all features and systems built into **CITY OF CHAOS** (built with **Gemini Argon**):

### 1. Open-World City & Dynamic Environment

* **Five Distinct Urban Districts**: Downtown Core with illuminated glass skyscrapers, North Hills and Southside residential suburbs, Sunset Beach & Pier with a boardwalk and oceanfront helipad, and the Industrial Harbor Zone with cargo yards across the canal.
* **Road Network & Active Traffic**: Multi-lane avenues and cross streets with yellow center dashes, crosswalks, streetlights, and 25+ intersections with automatic cycling red/green traffic lights.
* **Steel Suspension Bridges**: Three red steel suspension bridges connecting the Downtown mainland to the Industrial Harbor island across the canal waterway.
* **Five Walk-In Accessible Interiors**: Open-doorway buildings with custom wall-segment collision cutouts so you can walk directly inside **Vance Safehouse**, **Auto Customs**, **24/7 Tactical Armory**, **Metro Threads Clothing**, and the **Syndicate Warehouse Server Room**.
* **Four Weather & Lighting Presets**: Real-time toggle between **Golden Sunset**, **Neon Night**, **Rain Storm** (with 1,800 falling 3D rain particles and specular wet-road reflections), and **Clear Day**.
* **Living Pedestrian & Traffic AI**: 40 sidewalk pedestrians who walk, avoid obstacles, and panic/flee when gunfire erupts, alongside 26 moving traffic vehicles that obey red lights and brake for pedestrians or the player.

### 2. Third-Person Character & Controls

* **Articulated 3D Character Rig**: Custom procedural human character with animated limb swing cycles, torso crouch posture, customizable outfits, and a right-hand weapon attachment with dynamic muzzle flash.
* **Camera-Relative Movement & Physics**: Smooth third-person orbital camera with pointer-lock mouse look, gravity, jumping, sprinting, crouching, and sliding AABB collision resolution that prevents clipping into buildings or falling through bridges.

| Control / Key | On-Foot Action | Driving Action |
| --- | --- | --- |
| **`W` / `A` / `S` / `D**` | Walk / Strafe (camera-relative) | Accelerate, Reverse/Brake, and Steer |
| **`Mouse` / `Arrows**` | Rotate 3D camera & aim reticle | Orbit chase camera (auto-aligns at speed) |
| **`Shift`** | Sprint faster | — |
| **`Space`** | Jump over obstacles | Engage handbrake for high-speed drifts & tire skids |
| **`C`** | Toggle stealth crouch (lowers police detection range) | — |
| **`E`** | Enter nearby vehicle or interact with shop/terminal | Exit vehicle safely to the side |
| **`Left Click (LMB)`** | Fire equipped weapon (supports full-auto hold) | — |
| **`F`** | Perform close-quarters street melee attack | — |
| **`R` / `Q` / `1–5**` | Reload magazine / Cycle or select weapon slot | — |
| **`H`** | — | Honk vehicle horn |
| **`M` / `Tab` / `N` / `Esc**` | Open Full GPS Map / Gear & Garage Hub / Smartphone / Pause Menu | Same UI shortcuts |

### 3. Driving Physics & Vehicle Classes

* **Arcade-Realistic Handling**: Speed-sensitive steering, acceleration curves, braking, handbrake drift multiplier, chassis pitch under acceleration/braking, body roll in turns, illuminated brake lights, and persistent asphalt tire skid marks.
* **Chassis Damage & Collisions**: Vehicle-to-building and vehicle-to-vehicle collision responses with impact audio and health degradation.

| Vehicle Class | Top Speed (Base) | Chassis HP | Key Handling & Visual Traits |
| --- | --- | --- | --- |
| **Apex GT Sports** | 141 MPH | 140 HP | Aerodynamic low chassis, rear spoiler, rapid acceleration, tight drift control |
| **Vortex 900 Bike** | 150 MPH | 95 HP | Exposed rider posture, deepest cornering lean angle, fastest launch |
| **PD Interceptor** | 132 MPH | 200 HP | Black-and-white police livery, flashing red/blue roof lightbar, high-speed pursuit tuning |
| **Crown V8 Sedan** | 101 MPH | 160 HP | Balanced all-around street cruiser and starter garage vehicle |
| **Titan XL SUV** | 97 MPH | 240 HP | Heavy all-wheel stability and reinforced body armor |
| **Colossus Hauler** | 81 MPH | 340 HP | Heavy industrial cab able to ram through roadblocks |
| **Metro City Bus** | 75 MPH | 380 HP | Long-wheelbase transit coach with panoramic glass windows |

### 4. Five-Star Police & Wanted System

* **Witnessed Crime Escalation**: Commandeering occupied vehicles, firing weapons in public, assaulting NPCs, or ramming cruisers increases your Wanted Level from **1 ★ to 5 ★**.
* **Dynamic Police Pursuit**: Patrol cruisers actively navigate toward your live coordinates with flashing lightbars and wailing sirens, while foot officers deploy from cruisers to engage with firearms.
* **Tactical Bridge Roadblocks**: Reaching **4+ Wanted Stars** deploys police cruiser roadblocks and armed officers across main bridge approaches.
* **Line-of-Sight Evasion & Cooldown**: Breaking line-of-sight behind skyscrapers or crouching in alleys switches the HUD status from `PURSUIT ACTIVE` to `SEARCHING...`, filling an evasion bar from `0%` to `100%` to clear your stars and award a **+$250 Evasion Bonus**.

### 5. Story Campaign (6 Playable Missions)

All missions include live 3D glowing world beacons, radar GPS lines, multi-stage objectives, cash payouts, and automatic retry on failure:

| Mission | Objective Summary | Mechanics Featured | Reward |
| --- | --- | --- | --- |
| **1. First Ride** | Commandeer a vehicle and deliver it to Marco at Auto Customs Garage | Vehicle entry/exit & GPS waypoint navigation | **$1,500** |
| **2. The Delivery** | Pick up the marked Courier Sedan and deliver it to the Harbor Docks | Stealth driving (requires **0 ★ Wanted Level** and **>20% Car HP**) | **$2,500** |
| **3. Street Race** | Beat 3 AI-controlled sports car rivals through 6 city checkpoints | High-speed checkpoint racing & AI pathfinding | **$4,000** |
| **4. Getaway** | Survive Captain Cross's 3-Star ambush, break LOS, and return to the Safehouse | High-heat pursuit evasion & line-of-sight mechanics | **$5,000** |
| **5. The Warehouse** | Infiltrate the guarded Industrial Warehouse interior, steal the Data Drive, and cross the bridge | On-foot gun combat, interior infiltration, and getaway | **$6,500** |
| **6. Final Escape** | Hold position at the Broadcast Tower to upload the files, then survive a 4-Star lockdown to reach Sunset Pier Helipad | King-of-the-hill upload timer + 4-Star bridge roadblock gauntlet | **$15,000** |

### 6. Weapons & Tactical Combat

* **Hitscan & Multi-Pellet Ballistics**: 3D bullet tracer lines, spread cones, reload timers, hit-confirmation reticle markers, and enemy state transitions (`PATROL` → `ALERT` → `CHASE` → `COVER` / `ATTACK`).
* **Defeat & Medical Evac**: Depleting HP triggers the `WASTED` (or `BUSTED`) overlay before respawning you outside Vance Safehouse.

| Weapon | Damage | Range | Fire Mode & Magazine | Shop Price |
| --- | --- | --- | --- | --- |
| **Street Melee (`F` / Slot 1)** | 28 | 3.4m | Close-quarters punch swing (Infinite) | Starter |
| **9mm Tactical (`Slot 2`)** | 34 | 95m | Semi-auto sidearm (15 / 150) | Starter |
| **Viper SMG (`Slot 3`)** | 22 | 80m | High fire-rate automatic SMG (30 / 270) | **$650** |
| **Enforcer 12G (`Slot 4`)** | 24 × 6 pellets | 45m | Heavy pump shotgun spread (8 / 64) | **$1,100** |
| **Phantom AR (`Slot 5`)** | 42 | 135m | Long-range automatic assault rifle (30 / 240) | **$1,800** |

### 7. Economy, Customization & Progression

* **Auto Customs & Dealership**: Purchase any of the 7 vehicle classes for immediate delivery, apply **7 metallic paint swatches**, repair chassis damage (**$150**), or install **Stage 1–5 Turbo Engine Tuning** (**$600/level**) to boost top speed and acceleration.
* **24/7 Store & Metro Threads**: Buy Energy Packs (**+50 HP**), Heavy Kevlar (**100 Armor**), full ammo crates, and **5 unlockable character outfits** (*Street Racer*, *Tactical Night Ops*, *Sunset Neon Suit*, *Syndicate Executive*, *Gold Hazard Leather*).
* **Browser Save Persistence**: Automatically saves your cash balance, completed missions, unlocked weapons, owned vehicles, engine tuning level, and outfit to `localStorage` (with manual Save and Reset options).

### 8. GTA-Style HUD, Smartphone & Audio Engine

* **Rotating Circular Radar Minimap**: Displays roads, water, bridges, player heading cone, pulsing red/blue police units, hostile NPC blips, shop icons, and a dynamic dashed GPS line to your active mission or custom waypoint.
* **Interactive Full-Screen Satellite Map (`M`)**: Click anywhere on the city grid to drop a custom purple GPS pin or select 1-click landmark bookmarks.
* **In-Game Smartphone (`N`)**: Replay or jump to any of the 6 story missions on demand, or call contacts for instant field services—**Marco** (deliver a Sports Car for **$300**), **Elena** (bribe police to clear Wanted stars for **$800**), or **Arms Drop** (refill HP, Armor, and Ammo for **$500**).
* **Zero-Dependency Web Audio Synthesizer**: Real-time procedural sound effects using the browser's native Web Audio API for RPM-linked engine pitch, Doppler-style police sirens, distinct gunshots per weapon class, reload clicks, tire skids, car horns, crashes, footsteps, and cash rewards.
