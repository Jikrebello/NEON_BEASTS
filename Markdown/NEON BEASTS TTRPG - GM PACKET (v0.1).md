# NEON BEASTS TTRPG - GM PACKET (v0.1)

[TOC]

## Core combat procedure

This system lives or dies on pacing. If you run it like a slow tactical sim, the tone collapses. Your job is to keep turns snappy, keep the grid readable, and keep Hype moving.

### Round structure
Each Ranger turn: 2 Actions total. Typical: **Move** + **Action**, or spend Actions for bigger effects.
- **Move (1 Action):** move on the board, up to your full Move score.
- **Sprint (2** **Action):** use both actions on your turn to move up to your max Move score x2.
- **Attack (1 Action):** basic attack / setup move / utility. 
- **All-Out (2 Actions):** named attacks, weapon finishers, big wrestling moves.

```markdown
Double basic attack rule: you may attack twice, but your second basic is downgraded one step (Crit→Hit,Hit→Graze, Graze→Miss) and cannot Crit. This can be multi-targeted.
```

### Shot-clock (the 20-second rule)
If a player cannot decide within ~20 seconds:
- Default their turn to a **Basic Attack** or **Full Move to cover** (your pick).
- They lose **1 Personal Hype** (or if they are at 0, they become **Shaken**). 

### Cover, Ready, and Prone
- **Half Cover:** downgrade incoming ranged attacks by 1 step (Crit unaffected).
- **Full Cover:** cannot be targeted by ranged attacks unless repositioned/indirect/GM-approved angle.
- **Ready:** spend 1 Action to set a trigger (“If X happens, I do Y”). Fires later in the round when triggered (along with attack dice being rolled then).
- **Prone:** attacks against the target upgrade by 1 step for both melee and ranged. Some wrestling moves require Prone.

## Hype Economy (v0.1)

### Pools

- **Personal Hype (PH):** each Ranger max **2**
- **Team Hype (TH):** shared max = **5 + party size** (6 players → 11)

### Spending priority

- A move specifies **PH**, **TH**, or **Either**.
- If a move is “Either,” spend **PH first** unless the player explicitly chooses TH.

### Hard anti-loop rule

**You can gain at most:**

- **+1 Personal Hype per Ranger per round**, and
- **+2 Team Hype per round total** (party-wide cap).

This single cap prevents runaway “Hype factories” while still rewarding good play.

## Hype Gain Table

### Personal Hype (PH) gain

A Ranger gains **+1 PH** when they do any of the following (max +1 PH per Ranger per round):

1. **Named Hit:** You land a **Named move** on **Hit or Crit**.
   - (Graze does not count. Miss does not count.)
2. **Setup Conversion:** You create a **Tag Window** and an ally spends it to land a **Named move** before your next turn.
   - (You get +1 PH; the ally still gets their own PH from Named Hit.)
3. **Clutch Save:** You prevent a teammate’s Hit/Crit from landing via a defensive tool (e.g., Black intercept downgrade, Pink PR Spin, Shield Token spend) **and** the downgraded result becomes **Graze or Miss**.
   - (This rewards “support” without needing damage.)

Notes:

- A Ranger may only claim **one** of these PH gains per round (the per-Ranger cap).

### Team Hype (TH) gain

The team gains **+1 TH** when any of the following happens (party cap: +2 TH per round total):

1. **Style Chain:** The team lands **two different Named moves** in the same round (by any Rangers).
   - Only counts once per round.
2. **Mook Sweep:** The team Downs **3+ mooks** in a single round.
   - Only counts once per round.
3. **Objective Win:** The team completes an encounter objective step (disarm device, rescue civilian, stop ritual progress, etc.).
   - GM awards this. Max once per round.

Optional (if you want more TH early):

- **First Blood:** +1 TH the first time in a fight that the team Cracks Armor on a Lieutenant/Boss. (Once per fight.)


### Pink’s Sponsored Shield refund

**Sponsored Shield refund:** If the Shield Token is spent before Pink’s next turn, gain **+1 TH**, but this **cannot** cause the party to exceed the **+2 TH per round** gain cap.

### What is Hype mechanically
- **PH** is for “my moment” (named consistency, personal tricks, reactions).
- **TH** is for “our moment” (Tag moves, big team finishers, protection plays).

This keeps the team cooperating without forcing uniform builds.

## Status Design Map
```
Core rule: each move should do ONE of these jobs
```

1. **Damage**
2. **Setup (create Tag Window / apply Prone/Grabbed/Staggered)**
3. **Control (hard lock, only after armor cracks)**
4. **Support (Hype/shields/upgrade steps)**
5. **Positioning (push/pull/launch, cover denial)**

`Avoid moves that do 3+ jobs at once.`

### Prone
`bread-and-butter setup`
**Who should apply it often:** Yellow, Green, Monster-class lieutenants
**Best delivery:** 1 Action setup or 2 Action finisher
**Why:** Prone upgrades attacks (melee+ranged) and fuels wrestling sequences.

```
Good on:
Leg sweep / trip
throws that end with slam
AOE shockwave with “knockdown on crit only”
```

### Grabbed
`enables Tag moves and specific wrestling`
**Who should apply it reliably:** Black, Red; some Monster-class
**Best delivery:** 1 Action setup (low damage)
**Why:** It creates “hold them still” moments and forces enemies to spend Actions.

```
Good on:
Clincher grab, net toss, chain yank
```

### Staggered 
`tempo disruption; keep rarer`
**Who should apply it:** Red, a few lieutenants
**Best delivery:** 1 Action setup with modest damage OR as a rider on a 2 Action named (not both)
**Rule:** should not be common, or it becomes the best status.

### Exposed 
`accuracy/crit fishing enabler`
**Who should apply it:** Blue, Princess-class, some Pink/Green tools
**Best delivery:** Ranged mark, elegant villain strike
**Why:** supports “set up then cash in” without hard control.

### Shaken 
`soft control; common`
**Who should apply it:** Many enemies; some Ranger support tools
**Best delivery:** AOE chip, intimidation moves
**Why:** reduces enemy spike without removing agency.

### Launch 
`hard reposition; the “wow” move`
**Who should apply it:** Red/Black via big wrestling; Princess on signature; Monster on AOE sometimes
**Best delivery:** 2 Action named or Tag move
**Important:** On bosses, only after at least 1 Armor Token cracked.

### Pin 
`hard control; rarest`
**Who should apply it:** Black (signature), some Tag moves
**Best delivery:** 2 Action named; requires target Grabbed or Prone
**Important:** On bosses, only after armor crack. Keep it scarce.

### Move templates
#### Solo wrestling templates
1. **Setup Grapple (1 Action):** small damage (`1d4+stat`) + Grabbed + Tag Window
2. **Trip (1 Action):** small damage + Prone + Tag Window
3. **Slam (2 Action named):** medium damage (`2d4+stat`) + Launch/Prone
4. **Submission (2 Action named):** medium damage + Pin (requires Grabbed/Prone)

#### Tag wrestling templates
1. **Hot Tag Strike (TH 2):** medium damage + Crack Armor on Hit
2. **Alley-Oop (TH 2):** Launch + Prone (positioning payoff)
3. **Combo Pose (TH 1):** upgrade next ally attack by 1 step + generate TH (careful with caps)

### Weapon templates
Weapons should mostly differentiate by:
```
damage die profile (2d4 vs 1d8)
range (melee vs ranged)
one signature status rider
```

Examples:
- Sword (Red): Exposed or Crack Armor on crit
- Tonfa (Yellow): Prone rider
- Blaster (Blue): Exposed rider
- Chain/Whip (Green): Pull + Tag Window
- Gauntlets (Black): Grabbed rider
- Staff (Pink): TH generation / setup

### Stand templates (Level 3 path)
Stands should be “mode shifts,” not extra turns.

Give each Stand:
- 1 passive
- 1 basic attack
- 1 named (2 actions)
- 1 utility (mark, shield, reposition, etc.)

`Keep it symmetrical so they’re easy to run.`

## Defense Profiles and expected damage

All attacks resolve with a single d20 roll that produces a result step: **Miss, Graze, Hit, Crit**. The defender’s Defense Profile defines which d20 ranges map to each step.

### Result steps
- **Miss:** 0 damage, no on-hit effects.
- **Graze:** half damage (round down) and no rider effects unless explicitly allowed.
- **Hit:** full damage plus normal riders.
- **Crit:** full damage plus +1 damage die (or +50% for very small dice pools) plus crit riders.

### Defense Profiles
| **Profile**  | **Miss** | **Graze** | **Hit** | **Crit** | **Use for**                   |
| ------------ | -------- | --------- | ------- | -------- | ----------------------------- |
| **Easy**     | 1        | 2–4       | 5–19    | 20       | Mooks you want deleted fast   |
| **Standard** | 1–4      | 5–7       | 8–19    | 20       | Most Rangers, most Elites     |
| **Agile**    | 1–5      | 6–8       | 9–19    | 20       | Fast Rangers, slippery elites |
| **Tough**    | 1–3      | 4–7       | 8–19    | 20       | Tank Rangers, armored enemies |
| **Boss**     | 1–7      | 8–11      | 12–19   | 20       | Bosses before Armor breaks    |

### Tuning knobs
- If fights are too slow: reduce enemy HP (first), then reduce Armor Tokens (second), then widen Hit bands (third).

- If fights are too swingy: increase Graze bands and reduce Crit riders.
- If mooks feel toothless: increase positioning riders (Shove, Shaken, Pin attempts) rather than raw damage.

## Enemy tiers

Enemies are built from tier templates. Pick a tier, pick a role, write 1–2 named moves, and you are done.

### Tier summary
| **Tier**                       | **HP** | **Defense**      | **Basic**  **Damage** | **Move** | **Notes**                                   |
| ------------------------------ | ------ | ---------------- | --------------------- | -------- | ------------------------------------------- |
| **Mook**                       | 6–10   | Easy             | 1d4 + 1               | 4–5      | 1-hit KO from big hits; dies to  Tag splash |
| **Elite Mook**                 | 12–16  | Standard/Agile   | 1d6 + 1               | 5–6      | Has 1 simple named move; can guard          |
| **Lieutenant**  **(Princess)** | 28–36  | Standard         | 1d6 + 3               | 6        | Duelist; 2–3 named moves                    |
| **Lieutenant**  **(Monster)**  | 30–40  | Tough            | 1d6 + 2               | 5        | Summons/boosts mooks; AOE                   |
| **Boss/BBEG**                  | 60–90  | Boss to Standard | 2d6 + 3               | 5        | Armor Tokens 3–5; phases                    |
## Armor Tokens (Lieutenant/Boss only)

Armor Tokens create a visible “breakthrough” moment and prevent round-1 stun-lock. They do two things: a **Hard Control Gate** at full armor and **Damage Mitigation** that tapers as armor breaks.

### Hard Control Gate
- *Full Armor only:* while the enemy is at *full* Armor Tokens (e.g., 3/3 or 2/2), it ignores hard control: *Pinned, Stagger, Launch*. Soft control (push/pull, hazards, Shaken/Exposed, Tag Windows) still works.
- *Once armor is cracked:* after the enemy has lost at least 1 token (e.g., 2/3 or 1/2), hard control can apply normally.

### Damage Mitigation (damage only)
Armor mitigation reduces **damage only**. The attack result still counts for riders and setups.

| **Armor State**         | **Damage Mitigation**                                        |
| ----------------------- | ------------------------------------------------------------ |
| **2+ tokens remaining** | Crit damage counts as Hit damage; Hit damage counts as  Graze damage; Graze damage becomes 0. |
| **1 token remaining**   | Crit damage counts as Hit damage. (Hit/Graze unchanged.)     |
| **0 tokens**            | No mitigation.                                               |

### Armor Reaction (token spend)
Once per round, when the villain would suffer Grabbed/Pin/Stagger/Launch, it may spend 1 token to choose ONE:

- **Shake It Off:** downgrade the effect (Launch→Shove 2; Stagger→Shaken; Pin→cannot move 2; Grab→ends end of villain’s next turn).
- **Counter-Pose:** immediately take a 1-Action Beat (move 2, shove 1, summon 1 mook, etc.).

```
Boss-only pacing option: a boss cannot lose more than 1 Armor Token per round.
```

## Mooks (role templates + quick stat blocks)

Mooks should be fast to run and should create movement puzzles. Give each encounter 2–3 mook roles at most.

### Standard mook block
| **Name**         | **__________**                                     |
| ---------------- | -------------------------------------------------- |
| **Tier**         | Mook or Elite Mook                                 |
| **HP**           | ____                                               |
| **Defense**      | Easy / Standard / Agile                            |
| **Move**         | ____ squares                                       |
| **Basic Attack** | 1 Action. Hit: tier damage. Crit: +1 die.          |
| **Role Ability** | One sentence. Runnable in 2 seconds.               |
| **Named Move**   | Optional. 2 Actions, or 1 Action + a strong rider. |

### Mook roles
| **Role**        | **Hook**             | **Ability (simple)**                                         | **Named Move (optional)**                               |
| --------------- | -------------------- | ------------------------------------------------------------ | ------------------------------------------------------- |
| **Striker**     | Runs at squishies    | If adjacent to an ally, upgrade its next attack by 1 step.   | DOGPILE: 2A, 2 mooks adjacent → 2d4 damage.             |
| **Guard**       | Protects lieutenants | If adjacent to VIP, downgrade first incoming attack against VIP by 1  step (once/round). | SHIELD LINE: 1A, grant Half Cover to adjacent ally.     |
| **Shooter**     | Chip from cover      | Ignores Half Cover on Crit.                                  | VOLLEY: 2A, line 6, 1d6 damage; Graze on Miss.          |
| **Controller**  | Moves you around     | On Hit+: shove 1 square.                                     | TRIPWIRE: 1A, place hazard; first to enter is Prone.    |
| **Support**     | Keeps mooks alive    | Once/round, remove Shaken from a mook within 3.              | BANNER POSE: 1A, grant Shield Token to a mook (max 1).  |
| **Boomer Tech** | Unsafe gadgets       | When reduced to 0 HP, explode for 1d4 to adjacent.           | PROTOTYPE  LASER: 2A, 2d6; on Miss self becomes Shaken. |

```markdown
Surrender rule: 
When the lieutenant is defeated, surviving mooks surrender and flee. They drop a context item (badge, part, keycard, weird loot) that tees up the next scene.
```

## Lieutenants (Princess-class and Monster-class)

Lieutenants are episode villains. Each lieutenant gets 2–3 named moves and 1 objective that changes the fight.

### Princess-class (Duelist) template
**Fantasy:** a singularly dangerous opponent. Self-focused kit. She wants to win the scene by humiliating the Rangers on camera.

| **Stat Block** | **HP** **28–36 -** **Defense** **Standard -** **Move** **6 -** **Armor Tokens** **1–2 -** **Basic Damage** **1d6+3** |
| -------------- | ------------------------------------------------------------ |
| **Objective**  | Score 2 ‘Signature Moments’: land a named hit on Red or  crack a Ranger’s Shield Token. Each success gives +1 step on her next attack  (max 2). |
| **Passive**    | ANTI-NEON AURA: Rangers within 2 squares lose 1 Team Hype when they  Miss (once/round total). |
| **Named 1**    | SMOG DASH: 2 Actions. Move 6 ignoring engagement. Attack  2d4+3. On Hit+: target becomes Shaken. |
| **Named 2**    | DISMISSIVE BACKHAND: 1 Action. 1d6+3. On Hit+: shove 2 and remove Tag  Window. |
| **Named 3**    | CENSOR STAMP: 2 Actions. 2d6+3. Req: target Exposed. On  Hit+: Crack Armor (Lieutenant/Boss) OR remove Shield Token (Ranger). |

### Monster-class (Summoner/Controller) template
**Fantasy:** a big creature with tools. It boosts mooks, controls space, and forces the Rangers to split attention.

| **Stat Block** | **HP** **30–40 -** **Defense** **Tough -** **Move** **5 -** **Armor Tokens** **1–2 -** **Basic Damage** **1d6+2** |
| -------------- | ------------------------------------------------------------ |
| **Objective**  | Maintain a ‘Pack’ of 3+ mooks on the board. While the Pack  exists, the monster gains +1 step on basic attacks. |
| **Passive**    | OLD-SCHOOL BENEFITS: once per round, heal a mook for 4 HP.   |
| **Named 1**    | CALL THE CREW: 1 Action. Summon 2 mooks in open squares  within 3 (max 2 uses/fight). |
| **Named 2**    | AREA SWING: 2 Actions. 2d4+2 in a 3x3. On Hit+: Prone.       |
| **Named 3**    | MONSTER  SYNERGY: 1 Action. Choose a mook; it immediately takes a basic attack (out of  turn). |

```
Lieutenant defeat payoff: 
When the lieutenant drops, mooks surrender and the Rangers recover a scene-appropriate reward.
```

## Example Princess Class Lieutenants

### Princess Class 1: **SMOG PRINCESS**
**Type:** Duelist / Assassin

**Lieutenant Defense:** (Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20)

**Vibe:** glamorous villain in a soot-black cape with neon-killing haze; sincere, dramatic, and weirdly polite.
**Objective (pick one):**

- **Steal the Core:** end a turn adjacent to the objective and spend 1 Action to “secure it,” then escape next round.
- **Blackout the Broadcast:** reach 2 “camera nodes” and spend 1 Action at each (2 total successes).

**Failure consequence (if she succeeds):** next session starts with **Team Hype −2** (PR hit) or **one Sponsor Perk locked** for that mission.

#### Stats
```
HP: 35 | Armor Tokens: 1 | Move: 6 | Defense: Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20
```

#### Attacks
**1) Soot Fang (Basic Attack, 1 Action, melee)**
Damage: `1d6 + 2`
On Hit+: target becomes **Exposed** *(neon haze “marks” them)*

**2) Haze Step (Mobility, 1 Action)**
Move up to **4 squares** ignoring engagement/adjacency constraints (she can slip past).
If she ends adjacent to a target, she may make a **Soot Fang** as part of this action, but that attack is **downgraded 1 step** (keeps it fair).

**3) CHOKE THE NEON (Signature, 2 Actions, All-Out)**
Callout (she says it, of course): “CHOKE THE NEON!”
Make a melee attack against one target.
Damage on Hit+: `2d4 + 2`
On Hit+: target becomes **Shaken** *(next attack downgraded 1 step)*
On Crit: +1 die and the target is also **Prone**.

#### Reaction (once per round)
**Smog Veil (Reaction)**
Trigger: she is Hit or Crit by a Ranger attack.
Effect: Spend her **Armor Token** to downgrade that result by **1 step**.
If that reduces it to Miss, she may move **1 square** after the attack resolves.

#### AI script
- If she can score objective progress safely: do it (she’s an assassin, not a slugger).
- If a Ranger is isolated: **Haze Step** → **CHOKE THE NEON**.
- Otherwise: Basic attack + reposition to threaten the backline.

#### Defeat / retreat / drop
**On defeat:** she drops a smoke bomb, bows, and retreats (“Another day for the neon to breathe.”).
**Morale Break:** all mooks under her command surrender or scatter.

**Drop (Episode Loot Card): “SMOG CANISTER” (one-use)**

- **1 Action:** create a 3×3 cloud zone within 6 squares until end of round.
  - Enemies inside are **Shaken**.
  - Rangers inside gain **Half Cover** from ranged attacks.
- Compliance gag: you must announce “AIR QUALITY EVENT!” to deploy it.


### Princess Class 2: **STATIC PRINCESS**
**Vibe:** crackling anti-neon interference; moves look like “signal tearing.”
**Objective (pick 1):**

- **Cut the Feed:** spend 1 Action at **2 relay nodes** (two successes).
- **Steal the Callout:** tag 3 Rangers with Static (see move) then retreat.

**Failure consequence:** next fight starts with **Team Hype cap −2 for that mission** (signal interference).

#### Stats
```
HP: 35 | Armor Tokens: 1 | Move: 6 | Defense: Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20
```

#### Kit
**1) Arc Slash (Basic, 1 Action, melee)**
Damage `1d6+2`
On Hit+: target becomes **Shaken**.

**2) Signal Tag (1 Action, range 6)**
No damage. On Hit+: apply **Static Mark** (a simple tag):

- The next time that Ranger uses a Named move, it is downgraded 1 step **unless** they spend +1 Personal Hype.

**3) DEAD AIR (Signature, 2 Actions, All-Out)**
Pick up to **2 targets** within 2 squares of each other (melee or close range).
Attack both (one roll, apply results to both):

- On Hit+: each takes `1d4+2` and becomes **Exposed**.
- On Crit: +1 die to one target and that target is **Prone**.

#### Reaction (once/round)
**Flicker Step**
Trigger: hit/crit against her. Spend Armor Token to downgrade by 1 step; she teleports **2 squares**.

#### Drop
**“SIGNAL SCRAMBLER” (one-use)**
1 Action: Choose a target within 6. Until end of round, that target’s next attack is downgraded by 1 step (Crit unaffected).

### Princess Class 3: **RUST PRINCESS**
**Vibe:** corroded elegance; everything she touches “grinds.”
**Objective (pick 1):**

- **Corrode the Asset:** spend 1 Action adjacent to the objective for **2 rounds total**.
- **Break the Formation:** apply Prone/Grabbed to 2 Rangers in one fight (via moves).

**Failure consequence:** next mission, the team begins with **one random Ranger Shaken** (systems “grind” at start).

#### Stats
```markdown
HP: 35 | Armor Tokens: 1 | Move: 5 | Defense: Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20
```

#### Kit
**1) Corrosion Cut (Basic, 1 Action, melee)**
Damage `1d6+2`
On Hit+: target loses **1 Personal Hype** (if at 0, they become **Shaken**).

**2) Grind Hook (1 Action, melee)**
Damage `1d4+2`
On Hit+: **Grabbed**.

**3) OXIDE EXECUTION (Signature, 2 Actions, All-Out)**
Attack one Grabbed or Prone target:
Damage `2d4+2`
On Hit+: target becomes **Prone** (if not already) and **Exposed**.

#### Reaction (once/round)
**Rust Armor**
Spend Armor Token to downgrade one incoming Hit/Crit by 1 step. If reduced to Graze/Miss, she gains **+1 movement** next turn (Move 6 for a round).

#### Drop
**“ANTI-CORROSION COATING” (one-use)**
Reaction: When you would lose Personal Hype or become Shaken, ignore it and gain 1 Shield Token instead.


## Example Monster Class Lieutenants
### Monster Class 1: **CANNON BEAR**
**Type:** Mook Manager / Area Pressure
**Vibe:** big armored bear with a shoulder cannon; enthusiastic, dumb, and proud of his “crew.”
**Objective (pick one):**

- **Quota Run:** spawn **6 mooks** during the fight (doesn’t require them to survive).
- **Hold the Ground:** keep at least 1 of his mooks on a capture point for **3 rounds**.

**Failure consequence (if he succeeds):** next session begins with **+2 mooks** in the opening fight (the world remembers his “deployment success”).

#### Stats
```
HP: 35 | Armor Tokens: 1 | Move: 5 | Defense: Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20
Payroll cap: max 6 mooks
```

#### Rules: Payroll Cap
- Cannon Bear can have **at most 6 “on payroll” mooks** active at once.
- If he would spawn more, he instead upgrades 2 Fresh mooks to **Elite Mooks** (first Hit+ only Shakens them, second Hit+ downs them).

#### Attacks
**1) Maul Swipe (Basic Attack, 1 Action, melee)**
Damage: `1d6 + 2`

**2) CREW DEPLOYMENT (Summon, 1 Action)**
Spawn **2 mooks** in empty squares within 2 squares of Cannon Bear.
(Use your default mook statline; these are “his crew.”)

**3) CANNON SALUTE (Area, 2 Actions, All-Out, ranged cone/line)**
Pick either:

- a **3-square line** in sight, or
- a **2×2 blast** within 6 squares.
  Targets in the area take `1d4 + 1` on Hit+ and become **Shaken**.
  On Crit: +1 die (only to one target of your choice).

#### Reaction (once per round)
**Meat Shield (Reaction)**
Trigger: Cannon Bear is Hit or Crit by a Ranger attack and has a mook adjacent.
Effect: Redirect the attack to the adjacent mook.

- If it was a Hit/Crit, the mook goes **Down** (or **Shaken** if Elite).
- The attack does not affect Cannon Bear.

#### Aura (always on)
**Pack Spirit**
Mooks within 2 squares of Cannon Bear deal **+1 damage** on Hit+.
(That’s it. No stacking math.)

#### AI script (run fast)
- Early: **Crew Deployment** until he’s at 4–6 mooks.
- If Rangers cluster: **Cannon Salute**.
- If threatened: stay near mooks to enable **Meat Shield** and **Pack Spirit**.

#### Defeat / retreat / drop
**On defeat:** Cannon Bear howls, grabs his cannon core, and bolts into a tunnel/hatch.
**Morale Break:** all his mooks surrender immediately.

**Drop (Episode Loot Card): “CANNON CORE” (one-use)**

- **1 Action, ranged 6:** make an attack that **ignores Half Cover**.
  - On Hit+: deal `2d4` and **Crack Armor** (remove 1 token).
  - On Crit: +1 die.

### Monster Class 2: **HAMMER CROCODILE**
**Vibe:** big jaw + oversized hammer tail; loves knocking things down.
**Objective (pick 1):**

- **Hold the Waterline:** keep 2+ mooks adjacent to a marked zone for 3 rounds.
- **Break Their Legs:** make 3 targets Prone (via moves) in one fight.

**Failure consequence:** next mission, terrain starts with **2 hazard tiles** already active.

#### Stats
```
HP: 35 | Armor Tokens: 1 | Move: 5 | Defense: Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20
Payroll cap: max 6 mooks
```

#### Kit
**1) Tail Hammer (Basic, 1 Action, melee)**
Damage `1d6+2`
On Hit+: **Prone** (lieutenants can do this; bosses only after armor cracks as usual).

**2) Muck Call (1 Action)**
Spawn 2 mooks within 2 squares (respect payroll cap).

**3) SWAMP SLAM (Signature, 2 Actions, All-Out)**
2×2 blast within 4 squares:
On Hit+: `1d4+1` and **Shaken**.
On Crit: +1 die to one target and that target is **Prone**.

#### Reaction (once/round)
**Snap Counter**
Trigger: a Ranger ends movement adjacent to him.
Effect: make a basic attack against that Ranger (no All-Out).
(Once/round; this is how he punishes reckless dives.)

#### Drop
**“HAMMER TAIL MODULE” (one-use)**
1 Action, melee: On Hit+ deal `2d4` and force **Prone**.

### Monster Class 3: **DRILL BOAR**
**Vibe:** digs lanes, creates hazards, summons workers.
**Objective (pick 1):**

- **Tunnel Network:** create 3 Drill Tiles (see move) in one fight.
- **Escort the Payload:** a drill cart must reach an exit edge.

**Failure consequence:** next mission begins with **reduced cover** (arena “wrecked”).

#### Stats
```
HP: 35 | Armor Tokens: 1 | Move: 5 | Defense: Miss 1–3 / Graze 4–6 / Hit 7–18 / Crit 19–20
Payroll cap: max 6 mooks
```
#### Kit
**1) Gore Charge (Basic, 1 Action)**
Move 3 squares in a line, then attack:
Damage `1d6+2`
On Hit+: push 2 squares.

**2) Drill Tile (1 Action)**
Place a **Drill Tile** within 4 squares (max 3 tiles active).
Any character entering a Drill Tile becomes **Shaken** (once per turn).

**3) BORER BURST (Signature, 2 Actions, All-Out)**
Line 3 squares within 6:
On Hit+: `1d4+1`, **push 2**, and if pushed into a Drill Tile/wall they become **Prone**.

#### Reaction (once/round)
**Dig In**
Spend Armor Token to downgrade a Hit/Crit by 1 step. If downgraded, immediately place a Drill Tile adjacent to self.

#### Drop
**“BORER CHARGE” (one-use)**
1 Action: Move 3 in a straight line without provoking; then make a basic attack that ignores Half Cover.

## Encounter building

Use Threat Points (TP) to budget quickly. These numbers assume 4–5 Rangers. For 6 Rangers, add +15% TP.

### TP budgets
| **Fight Type**            | **Level 1** | **Level 2** | **Level 3** | **Notes**                       |
| ------------------------- | ----------- | ----------- | ----------- | ------------------------------- |
| **Trash (2–5 min)**       | 6–8         | 8–10        | 10–12       | Mostly mooks; 1 elite max       |
| **Mini-boss (8–12 min)**  | 10–12       | 12–14       | 14–16       | 1 lieutenant OR elite swarm     |
| **Set-piece (15–20 min)** | 14–16       | 16–18       | 18–22       | Lieutenants + mooks + objective |

### TP costs
| **Unit**                    | **TP** | **Notes**                           |
| --------------------------- | ------ | ----------------------------------- |
| **Mook**                    | 1      | HP 6–10, Easy defense               |
| **Shooter/Controller Mook** | 1.5    | If it has a strong shove/Prone tool |
| **Elite Mook**              | 2      | HP 12–16; 1 named move              |
| **Princess Lieutenant**     | 8      | Duelist; 1–2 Armor Tokens           |
| **Monster Lieutenant**      | 8      | Summons/boosts; 1–2 Armor Tokens    |
| **Boss/BBEG**               | 14+    | Use phases; Armor Tokens 3–5        |

### Objective templates
Pick an objective that forces movement and prevents a pure damage race:

- **Protect the sponsor van:** mooks try to tag the van 3 times.
- **Shut the vents:** 3 vents; interact (1 Action) to shut; each shut removes a hazard.
- **Capture the case:** monster carries a case; if it exits the map, Rangers lose the drop.
- **Hold the pose zone:** Rangers must control a marked tile for 2 rounds to complete the episode beat.

## Example encounters (Level 1–3)

### Level 1 – Trash sweep (6–8 TP)
**Setup:** 6 mooks (Striker + Shooter) in a small map with 2 Half Cover lanes.
**Beat:** Rangers clear quickly, build Team Hype, and end with a Tag finisher pose. **GM note:** if it ends too fast, add 2 reinforcement mooks on round 2.

### Level 2 – Princess duel (12–14 TP)
**Setup:** 1 Princess Lieutenant + 4 mooks. Armor Tokens: 2.
**Objective:** shut 2 vents. While vents are active, the first Ranger Miss each round costs -1 Team Hype. **Beat:** Princess tries to isolate a squishy target; Rangers must crack 1 token before hard control works.

### Level 3 – Big set-piece (18–22 TP)
**Setup:** Princess Lieutenant + Monster Lieutenant + 4 mooks. Tokens: Princess 2, Monster 2.
**Objective:** protect a sponsor kiosk for 2 rounds OR defeat either lieutenant.
**Beat:** Monster maintains a Pack; Princess hunts Red/Blue; Rangers coordinate Tag windows and armor cracks.
**Resolution rule:** When the first lieutenant drops, mooks surrender and the remaining lieutenant retreats unless you want a two-phase fight.

## Big Level 3 Episode Fight Example

### Encounter: **“Air Quality Incident”**
**Enemies:** Smog Princess + Cannon Bear + mooks
**Goal:** feels like a finale without being a 3-phase boss.

#### Why this works
- Princess forces precision decisions (protect backline/objective).
- Monster creates board pressure (mooks + aura + meat shields).
- Mooks provide pacing and spectacle.
- You can end it cleanly with Morale Break and retreats.

### Setup (6 PCs at Level 3)
#### Map
Medium map (roughly 12×12 squares). Include:
- 2–3 cover objects
- 1 raised platform or “broadcast tower”
- 1 “objective zone” in the middle (the Air Monitor / Core / Camera)

#### Starting positions
- Cannon Bear starts center-left with 2 mooks.
- Smog Princess starts far-right in partial cover.
- 4 additional mooks start spread.

#### Enemy counts (default)
- **Smog Princess** (35 HP, 1 Armor)
- **Cannon Bear** (35 HP, 1 Armor)
- **6 mooks total on board at start**
  Cannon Bear can summon up to 6 on payroll; in this combined fight, reduce his payroll cap to **4** (important for speed).

### Encounter Objective (for both sides)
#### Villain objective

They win if they complete either:
- **Smog Princess** spends 1 Action at the objective for **2 total successes**, OR
- **Cannon Bear** spawns **4 mooks** during the fight (quota) and keeps 2 mooks alive at the end of round 4.

(These are achievable but stoppable.)

#### Ranger win conditions
- Defeat either lieutenant. When one goes down, **all their mooks surrender**.
- Defeat both for a “perfect episode” result.

### Special Episode Rule: Smog Zone (simple and on theme)
At the **end of each round**, place a 2×2 Smog patch on a random edge or pre-marked vent tile.

- Any character entering Smog becomes **Shaken** (once per turn).
- Smog disappears at end of the next round.

It pressures movement without adding math.

### AI script (keeps it under 20 minutes)
#### Round 1
- Cannon Bear: Crew Deployment (if under cap), then reposition near mooks.
- Smog Princess: Haze Step into a threatening lane; basic attack to Expose.

### Round 2–3
- If Rangers cluster: Cannon Salute.
- If a backliner is exposed or isolated: Smog Princess uses signature.

#### Round 4+
- If villains are behind: both pivot to objectives (force the “stop them now” moment).
- If villains are ahead: Princess retreats as soon as she hits objective success; Bear tries to preserve mooks.

### Difficulty knobs (use during play)
If the party is crushing:
- Give Smog Princess a **second** use of Haze Step per round **but** only as movement (no attack).
- Add 2 more mooks from vents at round end (once).

If the party is struggling:
- Reduce Cannon Bear’s payroll cap from 4 to **3**.
- Remove the Smog Zone end-of-round rule.
- Have Princess prioritize objective over damage (less lethal).

### Rewards (Drops)
If they beat both lieutenants:

- They get **both Drops** (Smog Canister + Cannon Core)
  If they beat only one:
- They get that Drop; the other retreats with “their property.”

Also: grant **+2 Team Hype at the start of next mission** as the “episode win” bonus.

## Boss framework and printable templates

When you introduce a true BBEG, keep the same rules but add scripted beats so it feels like a finale without turning into a slog.

### Boss phases
- **Phase 1 (Armor up):** Defense Boss, Armor Tokens 3–5. Control gated until 1 token breaks.
- **Phase 2 (Armor cracked):** Defense Standard. Boss gains 1 nasty named move. Hard control now works. 
- **Phase 3 (Desperation):** At 25% HP, boss gains +1 step on its first attack each round; Rangers gain +1 Team Hype per round (cap still applies).

**Scripting rule:** never give a boss more than 3 named moves in a fight. Swap the list when a phase changes.

### Printable blank stat block

| **NAME / THEME**              | **____________________________________________**       |
| ----------------------------- | ------------------------------------------------------ |
| **Tier**                      | Mook / Elite / Princess Lt / Monster Lt / Boss         |
| **HP**                        | _____                                                  |
| **Defense Profile**           | Easy / Standard / Agile / Tough / Boss                 |
| **Move**                      | _____                                                  |
| **Armor Tokens**              | _____                                                  |
| **Basic Attack**              | Damage dice: __________ Rider: __________              |
| **Named Move A**              | Cost: ___ Effect: ____________________________________ |
| **Named Move B**              | Cost: ___ Effect: ____________________________________ |
| **Named Move C**              | Cost: ___ Effect: ____________________________________ |
| **Objective / Win Condition** | ____________________________________________           |
| **Loot / Drop**               | ____________________________________________           |

## Turn Order Modes
### Turn Order Mode A: Side Initiative (Episode Spotlight)
**When to use:** you want the fastest combats and the cleanest teamwork sequencing.

#### Start of each round
1. One Ranger rolls **1d20 + Heart** (or just **1d20** if you want zero stat influence).
2. GM rolls **1d20** for the villains.
3. Higher roll gets **Spotlight** (acts first). Ties go to Rangers (more heroic pacing).

#### Acting
- The Spotlight side activates **all units** in **any order**.
- Then the other side activates **all units** in **any order**.
- End of round: resolve hazards, end-of-round statuses, and any “end of round” Hype changes.

#### Enemy grouping
- **Mooks activate in squads** (2–3 squads max). Each squad takes one group turn.
- **Lieutenants** act as one unit (2 Actions).
- **Bosses** act as one unit (2 Actions) + a Lair Action (below).

#### Villain Beats
Each lieutenant/boss gets **1 Beat per round** (mooks don’t).
A Beat is a **single 1-Action effect** used outside their normal activation, triggered by an obvious “episode moment.”

Recommended triggers:

- After the first Ranger Crit of the round
- Immediately after a Tag Move resolves
- When a mook dies within 2 squares of the lieutenant
- When the lieutenant loses an Armor Token

Example Beats:
- **Reposition 2** (push/pull self or target)
- **Guard Pose** (downgrade the next incoming attack vs them by 1 step)
- **Summon 1 mook** (if Monster-class)
- **Taunt** (force a nearby Ranger to lose 1 Personal Hype on a Miss next turn)

#### Boss Lair Action
At **end of the round**, a boss can do one “environment move”:

- Spawn 2 mooks
- Place a hazard tile
- Force a shove/pull 2 from a marked tile
- Remove one Tag Window on them

This adds tension without adding a second boss turn.

### Turn Order Mode B: Speed Slots (XCOM Tempo)
**When to use:** you want speedsters to *always* matter and you want a consistent combat rhythm.

#### Everyone has a Speed Tier
- **Fast:** Yellow, Green
- **Normal:** Red, Pink
- **Slow:** Blue, Black
  (Enemies also have Fast/Normal/Slow.)

#### Round order
1. *Fast Rangers*
2. **Fast Enemies**
3. *Normal Rangers*
4. **Normal Enemies**
5. *Slow Rangers*
6. **Slow Enemies**
7. ***End of round cleanup***

#### Acting inside a slot
Within each slot, that side chooses activation order freely.

#### Enemy grouping
- Mooks are still 2–3 squads.
- Lieutenants are single units.
- Bosses are single units + optional Lair Action.

#### Why this doesn’t slow teamwork
Because order within each slot is free, you can still do:

- “Green sets Tag Window → Yellow capitalizes”
  as long as they’re both Fast (or you plan across slots).

### Shared rule for both modes: Ready/Hold
**Ready (1 Action):** declare a trigger and an action.

- Trigger resolves later in the round when it happens.
- You must still have valid range/LoS when it triggers.
- If the trigger never happens, the action is lost (keeps it from being strictly optimal play).

This is the “bridge” mechanic that makes both A and B support tag-team timing.

#### “No Perfect Lock” rule for bosses

Bosses and lieutenants cannot lose more than **1 Armor Token per round** (unless it’s a finale or you explicitly want a melt).

- This prevents optimized teams from deleting the set-piece before it becomes cinematic.

Below is a **generic Stand template kit** that turns your three archetypes (Sentinel / Artillery / Choreographer) into **reusable design patterns**. The intent is: you can invent a new Stand in 10 minutes, it will be balanced “enough” for v0.1, and it will still feel like a proto-Zord without adding turns.

## Stand Template Rules

**Stand = Mode, not a creature**
- A Stand never adds an extra turn or unit.
- While manifested, the Ranger uses normal actions as usual.

### Manifest
**Cost:** 1 Action
**Hype:** 1 Personal
**Duration:** until end of fight (or dismiss out of combat as flavor)
**Limit:** 1 Stand specialization per Ranger.

### Baseline Dice
- **Stand Basic:** `1d6 + (Tech or Heart or Power)`
- **Setup Named:** `2d4 + Stat` (reliable, lower spike)
- **Payoff Named:** `2d6 + Stat` (big moment)
- **Crit:** add **+1 die** to the damage roll.

### Boss control lock 
Launch/Pin/Stagger effects only apply after ≥1 Armor Token is cracked.

### Design constraint 
A Stand should have exactly:

- **Passive (once/round max)**
- **Basic (1 Action)**
- **Utility (1 Action)**
- **Named Setup (2 Actions)**
- **Named Payoff (2 Actions)**


### Stand Creation Worksheet
#### Pick the Stand’s Role 

`(choose ONE primary)`

- **Tank/Guard/Control** (Sentinel pattern)
- **Ranged/Mark/Armor Crack** (Artillery pattern)
- **Control/Reposition/Hype Engine** (Choreographer pattern)

Then pick ONE secondary theme:
- mobility
- debuffing
- shields
- multi-target
- anti-cover
- anti-mook
- duelist etc.

#### Choose the Stand’s Stat Axis
Pick one primary stat for most moves:

- **Power** (melee pressure / grapples / slam)
- **Tech** (ranged / gadgets / precision)
- **Heart** (support / staging / hype)

You can reference a second stat on exactly **one** move at most.

#### Define the Stand’s Passive 

`(once per round)`

Passives should do one of these:

- Generate **1 Personal Hype** (rare) OR **+1 Team Hype** (gated by cap) OR
- Enable a small positional move (step 1, shove/pull 1) OR
- Add a single “rider” when a specific condition happens.

**Hard rule:** passive triggers **once per round** and never adds more than
- +1 PH, or
- +1 TH, or
- 1 small movement, or
- 1 minor status like Shaken/Exposed **only on a named hit**.

#### Define Basic 

`(1 Action)`

Basic should be your “always okay” move:

- **Damage:** `1d6 + Stat`
- Optional rider on Hit+:
  - **push/pull 1**, or
  - apply **Shaken** OR **Exposed** (not both), or
  - ignore Half Cover under a condition (e.g., “if you didn’t move”).

**Hard rule:** Basic should not Crack Armor and should not grant Tag Window by itself unless it’s very conditional.

#### Define Utility 
`(1 Action)`

Utility must do **one** job, clearly:

- grant an ally Half Cover / Shield Token (cap 1)
- apply Exposed / Tag Window at range (costly)
- reposition someone 1–2 squares
- remove Shaken from an ally
- create a hazard tile / spotlight zone

**Hype gating:**

- If Utility gives defense to allies (Shield Token), it should cost **1 Team Hype**.
- If Utility creates Tag Window at range, it should cost **1 Personal Hype** (or 1 Team Hype if it’s very strong).

#### Named Setup

 `(2 Actions)`

Setup Named is the “I’m creating the episode beat.”

- **Damage:** `2d4 + Stat`
- On Hit+ apply **one major setup**:
  - Tag Window, OR
  - Prone, OR
  - Grabbed (if allowed by armor state), OR
  - Shaken + Exposed (counts as one package for Artillery-style)
- Often includes a reposition effect (pull 2, shove 2).

**Hard rule:** Setup Named should not Crack Armor unless it’s the Stand’s entire identity and the payoff does something else.

#### Named Payoff 

`(2 Actions)`

Payoff is the “finisher moment.”

- **Damage:** `2d6 + Stat`
- On Hit+ does **one** of:
  - Launch (push 3) + Prone, OR
  - Crack Armor, OR
  - AOE hit (small area), OR
  - Big single-target + forced move

**Hard rule:** Payoff should have a **requirement** (so it’s not spam):

- target is Grabbed or Prone, OR
- target is Exposed, OR
- target has Tag Window, OR
- you did not move this turn, etc.

### The Three Archetype Templates

#### Template A: SENTINEL Pattern 
`Tank / Guard / Control`

- **Passive (1/round):** reward defense play (Shield Token spent, successful downgrade, ally protected). Gain +1 PH or a free step.
- **Basic:** `1d6 + Power`, on Hit+ push 1.
- **Utility:** defensive support (Half Cover + Shield Token cap 1) costing **1 Team Hype**.
- **Named Setup:** `2d4 + Power`, on Hit+ Grabbed + Tag Window (or Pin if armor cracked).
- **Named Payoff:** `2d6 + Power`, requires Grabbed/Prone; on Hit+ Launch + Prone; on Crit optionally Crack Armor.

**Balance flags to avoid:**

- Don’t give free Shield Tokens with no Team Hype cost.
- Don’t allow Grabbed before armor crack unless you explicitly want “anti-boss” tech.

#### Template B: ARTILLERY Pattern 
`Ranged / Mark / Armor Crack`

- **Passive (1/round):** reward applying Exposed/marking. +1 Team Hype if cap allows.
- **Basic:** `1d6 + Tech`, conditional Half Cover ignore if you didn’t move.
- **Utility:** Lock-on mark: on Hit+ apply Exposed + Tag Window, costing **1 Personal Hype**.
- **Named Setup:** `2d4 + Tech`, on Hit+ Shaken + Exposed (the “set them up”).
- **Named Payoff:** `2d6 + Tech`, costs 2 Team Hype; on Hit+ Crack Armor (and maybe Prone on Crit).

**Balance flags to avoid:**

- Don’t let basic attacks Crack Armor.
- Keep Crack Armor mostly on the Payoff named.

#### Template C: CHOREOGRAPHER Pattern 
`Control / Reposition / Hype Engine`

- **Passive (1/round):** when an ally lands a Named Hit, you get a free 1-step reposition; optionally gain +1 PH if you “get into position.”
- **Basic:** `1d6 + Heart`, on Hit+ optional pull 1.
- **Utility:** “Cue” an ally (upgrade next attack by 1 step OR grant Shield Token), costing **1 Team Hype**.
- **Named Setup:** `2d4 + Heart`, on Hit+ pull 2 + Prone + Tag Window.
- **Named Payoff:** `2d6 + Heart`, requires Tag Window; on Hit+ choose Launch+Prone OR Crack Armor.

**Balance flags to avoid:**

- Don’t make the Utility both an upgrade and a shield at once.
- Don’t give free team-wide upgrades without Team Hype.


### Quick Stand Balance Checklist (v0.1)

Before approving a new Stand, check:
1. Does it **add no extra turns**? (must be yes)
2. Does it have **exactly one** Crack Armor source (usually the Payoff named)?
3. Does it have **a requirement** on the Payoff named?
4. Does it avoid giving **free Shield Tokens** (should cost Team Hype)?
5. Does it generate no more than **+1 Hype/round** from passive?
6. Can it do **setup + payoff** in a single turn? (should generally be **no** unless it’s spending big Team Hype and positioning was pre-done)

### Example Blank Stand Sheet
Use this to create a new Stand in one page:

**Stand Name:** ________
**Fantasy:** ________
**Best for:** ________
**Stat Axis:** Power / Tech / Heart

**Manifest:** 1 Action, 1 Personal Hype, lasts fight

**Passive (1/round):** ________
**Basic (1A):** Damage `1d6 + ___` | On Hit+: ________
**Utility (1A):** Range ___ | Cost: ___ Hype | Effect: ________
**Named Setup (2A):** Damage `2d4 + ___` | On Hit+: ________
**Named Payoff (2A):** Req: ________ | Cost: ___ Hype | Damage `2d6 + ___` | On Hit+: ________ | On Crit: ________
