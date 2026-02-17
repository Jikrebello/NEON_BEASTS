# NEON BEASTS TTRPG - PLAYER PACKET (v0.1)

[TOC]

<br/>

## Core Play Loop

1. You fight on a grid. Positioning and teamwork create Tag Windows.
2. Most turns are: Move + Action. If you do not move, you can All-Out or Sprint for 2 Actions.
3. Named moves spend Hype and deliver the big show moments.
4. Bosses use Armor Tokens; crack armor first, then land hard control and finishers.

### Turn Structure and Movement
On your turn you may Move up to your Move value (squares) and take 1 Action.

- Sprint: spend your Action to Move again (double your Move).
- All-Out: if you do not Move this turn, you gain 2 Actions instead of 1.
- Double basic attacks (All-Out): the second basic attack is downgraded 1 step and cannot Crit.

| **Ranger Color** | **Move** | **Sprint (Action)** |
| ---------------- | -------- | ------------------- |
| Yellow           | 6        | 12                  |
| Green            | 6        | 12                  |
| Red              | 5        | 10                  |
| Pink             | 5        | 10                  |
| Black            | 4        | 8                   |
| Blue             | 4        | 8                   |

Prone stand-up options:
- Quick Stand: spend 2 squares of movement to stand, keep your 2nd Action.
- Full Reset: spend 1 Action to stand, keep full movement.

### Attacks, Defense Bands, and Damage
Attacks roll a d20 and consult the target's defense band: Miss, Graze, Hit, Crit.

- Graze: half damage (round down). Unless a move explicitly says otherwise, grazes do not apply status riders.
- Crit: full damage + add 1 bonus damage die (same die size as the attack).
- Cover affects ranged attacks (see Section 4).

| **Target Type**              | **Miss** | **Graze** | **Hit** | **Crit** |
| ---------------------------- | -------- | --------- | ------- | -------- |
| Mook (when you attack)       | 1        | 2-4       | 5-19    | 20       |
| Lieutenant (when you attack) | 1-3      | 4-6       | 7-18    | 19-20    |
| Boss (when you attack)       | 1-5      | 6-8       | 9-18    | 19-20    |
| **Ranger Defense Profile**   | **Miss** | **Graze** | **Hit** | **Crit** |
| Agile                        | 1-5      | 6-8       | 9-19    | 20       |
| Standard                     | 1-4      | 5-7       | 8-19    | 20       |
| Armored                      | 1-3      | 4-8       | 9-19    | 20       |

### Grid Rules, Cover, and Ready
Cover is intentionally minimal:

- Half Cover: downgrade ranged results by 1 step (Crit unaffected).
- Full Cover: cannot be targeted by ranged attacks unless repositioned, indirect/arching, or suppressed.
- Ready (Hold): spend 1 Action to declare a trigger. When triggered later in the round, you perform the readied action if you still have line of sight/range.

### Status Conditions
- **Exposed:** next incoming attack upgrades by 1 step.
- **Shaken:** your next attack is downgraded by 1 step.
- **Staggered:** you lose 1 Action next turn (cannot All-Out that turn).
- **Grabbed:** your movement is 0. Break free costs 1 Action.
- **Pinned:** like Grabbed, plus you cannot Quick Stand. Break free costs 1 Action. (Hard control; rare.)
- **Launched:** pushed 3 squares and becomes Prone.
- **Prone:** attacks against you upgrade by 1 step (melee and ranged).
- **Tag Window:** enables Tag-Team moves against that target until the start of the creator's next turn (only 1 Tag Window per target at a time).

### Armor Tokens and Control Lock
- Lieutenants typically have 1 Armor Token. Bosses have Armor Tokens per phase.
- Crack Armor removes 1 token on Hit+ (as specified by a move).
- Boss control lock: Launch/Pin/Stagger only apply to bosses after at least 1 Armor Token has been cracked. Damage still applies normally.

### Hype Economy (v0.1)
Hype fuels Named moves and teamwork. Hype gains are capped to prevent runaway loops.

- Personal Hype (PH): each Ranger max 2.
- Team Hype (TH): shared max = 5 + party size (6 players -> 11).
- Gain caps: max +1 PH per Ranger per round; max +2 TH per round party-wide.

#### Personal Hype gain
- Named Hit: you land a Named move on Hit or Crit (not Graze).
- Setup Conversion: you create a Tag Window and an ally spends it to land a Named move before your next turn.
- Clutch Save: you downgrade an incoming Hit/Crit on an ally to Graze or Miss using a defensive tool (Shield, PR Spin, intercept, etc.).
	
#### Team Hype gain (party cap +2 TH per round)
- Style Chain: two different Named moves land in the same round (once per round).
- Mook Sweep: 3+ mooks go Down in one round (once per round).
- Objective Win: you complete an encounter objective step (GM award; once per round).

Shield Tokens: a Ranger may hold at most 1 Shield Token. Spend it when attacked to downgrade the incoming result by 1 step (Crit -> Hit -> Graze -> Miss).

<br/>

## Universal Wrestling Moves (v0.1)

All Rangers can use these moves. Most setups create Tag Windows; Tag moves are the payoff.

### Solo Moves

| **Move**           | **Cost**           | **Damage**    | **On Hit+ (and other notes)**                                |
| ------------------ | ------------------ | ------------- | ------------------------------------------------------------ |
| Clincher Grab      | 1 Action           | 1d4 + Power   | Grabbed + Tag Window.                                        |
| Leg Sweep          | 1 Action           | 1d4 + Agility | Prone + Exposed + Tag Window.                                |
| Shoulder Check     | 1 Action           | 1d4 + Power   | Staggered + Tag Window.                                      |
| Irish Whip         | 1 Action           | 1d4 + Heart   | Push 2; if ends adjacent to an ally, Tag Window.             |
| Rope-a-Dope        | 1 Action           | 1d4 + Heart   | Shaken. If target already Shaken, also Tag Window.           |
| Feint & Snap       | 1 Action           | 1d4 + Agility | Tag Window; your next attack vs target this round upgrades  by 1 step. |
| Powerbomb Protocol | 2 Actions + 1 Hype | 2d4 + Power   | Launch (push 3) + Prone.                                     |
| Submission Hold    | 2 Actions + 1 Hype | 1d6 + Power   | Pinned (requires target Grabbed or Prone).                   |
| Meteor Swing       | 2 Actions + 1 TH   | 1d6 + Power   | Requires Grabbed. Prone. Adjacent enemies take 1d4 graze  damage. |
| Ring-Out Throw     | 2 Actions + 1 TH   | 1d6 + Heart   | Push 4; collision adds +1d4 and Prone.                       |

### Tag-Team Moves
- Requirements: target has a Tag Window; two Rangers participate; each spends 1 Action in the same round.
- Position: both adjacent to target, or one adjacent + one within 2 squares with line of sight.
- Hype: one participant pays the Team Hype cost.


| **Move**              | **TH Cost** | **Damage**           | **On Hit+ (and other notes)**                                |
| --------------------- | ----------- | -------------------- | ------------------------------------------------------------ |
| One-Two Justice Combo | 1           | 2d4 + highest  Power | Upgrade the result by 1 step (for this tag attack).          |
| Hot Tag Clothesline   | 2           | 1d6 + 4              | Crack Armor (Lieutenant/Boss).                               |
| Alley-Oop Suplex      | 2           | 2d4 + 2              | Launch (push 3) + Prone.                                     |
| Turnbuckle Crash      | 2           | 2d4 + 2              | If slam into obstacle, +1d4; Shaken (Crit: Prone instead).   |
| Contract Termination  | 3           | 2d6 + 2              | Requires Staggered/Grabbed/Prone. On Hit+: remove 1 extra  Armor Token (total 2) or apply Exposed. |
| Stereo Finisher Pose  | 1           | -                    | No damage. Gain +2 TH (still obeys TH gain cap) and upgrade  next ally attack this round by 1 step. |

<br/>
## Weapon Packages (v0.1)

Each Ranger color has a signature weapon with a Basic attack and two Named attacks.

### Red - Solar Saber

| **Attack**       | **Cost**                  | **Damage**  | **Effect**                                                   |
| ---------------- | ------------------------- | ----------- | ------------------------------------------------------------ |
| Basic            | 1 Action, melee           | 1d6 + Power | Standard strike.                                             |
| SOLAR MARK SLASH | 2 Actions (All-Out), 1 PH | 2d4 + Power | Exposed + Tag Window. Crit: +1 die and Crack Armor  (Lt/Boss). |
| HELIOS CLEAVE    | 2 Actions (All-Out), 1 TH | 2d6 + Power | Hit+: Crack Armor (Lt/Boss). Optional graze splash to  adjacent target. |

### Yellow - Volt Tonfas

| **Attack**         | **Cost**                     | **Damage**    | **Effect**                               |
| ------------------ | ---------------------------- | ------------- | ---------------------------------------- |
| Basic              | 1 Action, melee              | 1d6 + Agility | Fast striker.                            |
| VOLT TRIP COMBO    | 1 Action, 1 PH               | 1d4 + Agility | Prone + Tag Window; then move 2 squares. |
| FLASHSTEP FINISHER | 2 Actions (All-Out), 1 PH/TH | 2d4 + Agility | Hit+: upgrade your result by 1 step.     |

### Blue - Glacier Blaster

| **Attack**            | **Cost**                  | **Damage** | **Effect**                                                   |
| --------------------- | ------------------------- | ---------- | ------------------------------------------------------------ |
| Basic                 | 1 Action, ranged          | 1d6 + Tech | Cover applies.                                               |
| GLACIER MARKER  ROUND | 1 Action, 1 PH            | 1d4 + Tech | Exposed + Tag Window.                                        |
| ZERO-LINE RAILSHOT    | 2 Actions (All-Out), 1 TH | 2d4 + Tech | Ignores Half Cover. Hit+: Crack Armor (Lt/Boss). Crit: +1  die + Shaken. |

### Green - Vine Chain

| **Attack**          | **Cost**                  | **Damage**  | **Effect**                                                   |
| ------------------- | ------------------------- | ----------- | ------------------------------------------------------------ |
| Basic               | 1 Action, melee/reach     | 1d6 + Heart | Control lash.                                                |
| VINE SNARE YANK     | 1 Action, 1 PH            | 1d4 + Heart | Pull 2 + Grabbed + Tag Window.                               |
| SERPENT SWING  SLAM | 2 Actions (All-Out), 1 TH | 1d6 + Heart | Requires Grabbed. Prone. Adjacent enemies take 1d4 graze  damage. |

### Black - Obsidian Gauntlets

| **Attack**          | **Cost**                  | **Damage**  | **Effect**                                                   |
| ------------------- | ------------------------- | ----------- | ------------------------------------------------------------ |
| Basic               | 1 Action, melee           | 2d4 + Power | Heavy hits.                                                  |
| RHINO CLINCH        | 1 Action, 1 PH            | 1d4 + Power | Grabbed + Staggered + Tag Window (if too strong in  playtests, drop Stagger). |
| OBSIDIAN PILEDRIVER | 2 Actions (All-Out), 1 TH | 2d6 + Power | Requires Grabbed/Prone. Launch + Prone. Crit: +1 die +  Crack Armor (Lt/Boss). |

### Pink - Starlight Bow

| **Move**                              | **Cost**                 | **Damage** | **Effect**                                                   |
| ------------------------------------- | ------------------------ | ---------- | ------------------------------------------------------------ |
| Basic                                 | 1 Action, ranged         | 1d6 + Tech | Cover applies.                                               |
| **BRANDED  STRIKE SHOT**  **Support** | 1 Action,                | 2d4 + Tech | Make a ranged attack. Upgrade the result by **1 step** (Miss→Graze→Hit→Crit).  Damage **1d6 + Tech**. |
| **HEARTBEAT  VOLLEY**  **Payoff**     | 2 Actions (All-Out), 1TH | 2d4 + Tech | Damage **2d4 + Tech**.  On Hit+: choose one ally within 3 squares:  they gain a **Shield  Token** (max 1) OR remove **Shaken**. |

<br/>
## Neon Avatars (Stands) v0.1

At Level 3, each Ranger manifests a mythic Neon Avatar. Each color has two locked options.
```markdown
All Neon Avatars share: Manifest (1 Action + 1 Personal Hype), no separate turn, and the Boss Control Lock.
```

### Red - Unicorn Avatar

#### Option A: Unicorn Sentinel

- **Passive:** Once per round, when you downgrade an incoming attack (Shield/PR Spin/intercept/etc.), gain +1 Personal Hype (PH cap applies).

- **Basic:** Horn/Claw Strike (1 Action, melee): 1d6 + Power; on Hit+ push 1.

- **Utility:** Aegis Guard (1 Action, range 3, Team Only, cost 1 Team Hype): grant Half Cover + Shield Token (max 1) until your next turn.

- **Named 1:** Lock Move (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Power; on Hit+ Grabbed + Tag Window.

- **Named 2:** Verdict Slam (2 Actions All-Out, cost 1 Team Hype; requires Grabbed/Prone): 2d6 + Power; on Hit+ Launch (push 3) + Prone; on Crit +1 die and Crack Armor (Lt/Boss).

#### Option B: Unicorn Artillery

- **Passive:** Once per round, when you apply Exposed, gain +1 Team Hype (obeys +2 TH/round cap).

- **Basic:** Beam/Bolt (1 Action, ranged): 1d6 + Tech. If you did not Move this turn, ignore Half Cover.

- **Utility:** Lock-On (1 Action, range 8, cost 1 Personal Hype): no damage; on Hit+ Exposed + Tag Window.

- **Named 1:** Freeze/Shear (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Tech; on Hit+ Shaken + Exposed.

- **Named 2:** Sunder Line (2 Actions All-Out, cost 2 Team Hype): 2d6 + Tech; on Hit+ Crack Armor; on Crit +1 die and Prone (if eligible).

### Blue - Cyclops Avatar

#### Option A: Cyclops Artillery

- **Passive:** Once per round, when you apply Exposed, gain +1 Team Hype (obeys +2 TH/round cap).

- **Basic:** Beam/Bolt (1 Action, ranged): 1d6 + Tech. If you did not Move this turn, ignore Half Cover.

- **Utility:** Lock-On (1 Action, range 8, cost 1 Personal Hype): no damage; on Hit+ Exposed + Tag Window.

- **Named 1:** Freeze/Shear (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Tech; on Hit+ Shaken + Exposed.

- **Named 2:** Sunder Line (2 Actions All-Out, cost 2 Team Hype): 2d6 + Tech; on Hit+ Crack Armor; on Crit +1 die and Prone (if eligible).

#### Option B: Cyclops Choreographer

- **Passive:** Once per round, when an ally lands a Named Hit, you may step 1 square for free. If this makes you adjacent to that target, gain +1 Personal Hype (PH cap applies).

- **Basic:** Tether Lash (1 Action, range 6): 1d6 + Heart; on Hit+ pull 1 (optional).

- **Utility:** Encore Cue (1 Action, range 3, Team Only, cost 1 Team Hype): upgrade ally's next attack this round by 1 step OR grant Shield Token (max 1).

- **Named 1:** Stage Reset (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Heart; on Hit+ pull 2 + Prone + Tag Window.

- **Named 2:** Finale Pull (2 Actions All-Out, cost 1 Team Hype; requires Tag Window): 2d6 + Heart; on Hit+ choose Launch+Prone OR Crack Armor.

### Yellow - Griffin Avatar

#### Option A: Griffin Choreographer

- **Passive:** Once per round, when an ally lands a Named Hit, you may step 1 square for free. If this makes you adjacent to that target, gain +1 Personal Hype (PH cap applies).

- **Basic:** Tether Lash (1 Action, range 6): 1d6 + Heart; on Hit+ pull 1 (optional).

- **Utility:** Encore Cue (1 Action, range 3, Team Only, cost 1 Team Hype): upgrade ally's next attack this round by 1 step OR grant Shield Token (max 1).

- **Named 1:** Stage Reset (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Heart; on Hit+ pull 2 + Prone + Tag Window.

- **Named 2:** Finale Pull (2 Actions All-Out, cost 1 Team Hype; requires Tag Window): 2d6 + Heart; on Hit+ choose Launch+Prone OR Crack Armor.

#### Option B: Griffin Sentinel

- **Passive:** Once per round, when you downgrade an incoming attack (Shield/PR Spin/intercept/etc.), gain +1 Personal Hype (PH cap applies).
- **Basic:** Horn/Claw Strike (1 Action, melee): 1d6 + Power; on Hit+ push 1.

- **Utility:** Aegis Guard (1 Action, range 3, Team Only, cost 1 Team Hype): grant Half Cover + Shield Token (max 1) until your next turn.

- **Named 1:** Lock Move (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Power; on Hit+ Grabbed + Tag Window.

- **Named 2:** Verdict Slam (2 Actions All-Out, cost 1 Team Hype; requires Grabbed/Prone): 2d6 + Power; on Hit+ Launch (push 3) + Prone; on Crit +1 die and Crack Armor (Lt/Boss).

### Green - Hydra Avatar

#### Option A: Hydra Choreographer

- **Passive:** Once per round, when an ally lands a Named Hit, you may step 1 square for free. If this makes you adjacent to that target, gain +1 Personal Hype (PH cap applies).
- **Basic:** Tether Lash (1 Action, range 6): 1d6 + Heart; on Hit+ pull 1 (optional).
- **Utility:** Encore Cue (1 Action, range 3, Team Only, cost 1 Team Hype): upgrade ally's next attack this round by 1 step OR grant Shield Token (max 1).

- **Named 1:** Stage Reset (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Heart; on Hit+ pull 2 + Prone + Tag Window.
- **Named 2:** Finale Pull (2 Actions All-Out, cost 1 Team Hype; requires Tag Window): 2d6 + Heart; on Hit+ choose Launch+Prone OR Crack Armor.

#### Option B: Hydra Artillery

- **Passive:** Once per round, when you apply Exposed, gain +1 Team Hype (obeys +2 TH/round cap).

- **Basic:** Beam/Bolt (1 Action, ranged): 1d6 + Tech. If you did not Move this turn, ignore Half Cover.

- **Utility:** Lock-On (1 Action, range 8, cost 1 Personal Hype): no damage; on Hit+ Exposed + Tag Window.

- **Named 1:** Freeze/Shear (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Tech; on Hit+ Shaken + Exposed.

- **Named 2:** Sunder Line (2 Actions All-Out, cost 2 Team Hype): 2d6 + Tech; on Hit+ Crack Armor; on Crit +1 die and Prone (if eligible).

### Black - Minotaur Avatar

#### Option A: Minotaur Sentinel

- **Passive:** Once per round, when you downgrade an incoming attack (Shield/PR Spin/intercept/etc.), gain +1 Personal Hype (PH cap applies).
- **Basic:** Horn/Claw Strike (1 Action, melee): 1d6 + Power; on Hit+ push 1.

- **Utility:** Aegis Guard (1 Action, range 3, Team Only, cost 1 Team Hype): grant Half Cover + Shield Token (max 1) until your next turn.

- **Named 1:** Lock Move (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Power; on Hit+ Grabbed + Tag Window.

- **Named 2:** Verdict Slam (2 Actions All-Out, cost 1 Team Hype; requires Grabbed/Prone): 2d6 + Power; on Hit+ Launch (push 3) + Prone; on Crit +1 die and Crack Armor (Lt/Boss).

#### Option B: Minotaur Choreographer

- **Passive:** Once per round, when an ally lands a Named Hit, you may step 1 square for free. If this makes you adjacent to that target, gain +1 Personal Hype (PH cap applies).
- **Basic:** Tether Lash (1 Action, range 6): 1d6 + Heart; on Hit+ pull 1 (optional).

- **Utility:** Encore Cue (1 Action, range 3, Team Only, cost 1 Team Hype): upgrade ally's next attack this round by 1 step OR grant Shield Token (max 1).

- **Named 1:** Stage Reset (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Heart; on Hit+ pull 2 + Prone + Tag Window.

- **Named 2:** Finale Pull (2 Actions All-Out, cost 1 Team Hype; requires Tag Window): 2d6 + Heart; on Hit+ choose Launch+Prone OR Crack Armor.

### Pink - Phoenix Avatar

#### Option A: Phoenix Choreographer

- **Passive:** Once per round, when an ally lands a Named Hit, you may step 1 square for free. If this makes you adjacent to that target, gain +1 Personal Hype (PH cap applies).
- **Basic:** Tether Lash (1 Action, range 6): 1d6 + Heart; on Hit+ pull 1 (optional).

- **Utility:** Encore Cue (1 Action, range 3, Team Only, cost 1 Team Hype): upgrade ally's next attack this round by 1 step OR grant Shield Token (max 1).

- **Named 1:** Stage Reset (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Heart; on Hit+ pull 2 + Prone + Tag Window.

- **Named 2:** Finale Pull (2 Actions All-Out, cost 1 Team Hype; requires Tag Window): 2d6 + Heart; on Hit+ choose Launch+Prone OR Crack Armor.

#### Option B: Phoenix Sentinel

- **Passive:** Once per round, when you downgrade an incoming attack (Shield/PR Spin/intercept/etc.), gain +1 Personal Hype (PH cap applies).
- **Basic:** Horn/Claw Strike (1 Action, melee): 1d6 + Power; on Hit+ push 1.

- **Utility:** Aegis Guard (1 Action, range 3, Team Only, cost 1 Team Hype): grant Half Cover + Shield Token (max 1) until your next turn.

- **Named 1:** Lock Move (2 Actions All-Out, cost 1 Personal Hype): 2d4 + Power; on Hit+ Grabbed + Tag Window.

- **Named 2:** Verdict Slam (2 Actions All-Out, cost 1 Team Hype; requires Grabbed/Prone): 2d6 + Power; on Hit+ Launch (push 3) + Prone; on Crit +1 die and Crack Armor (Lt/Boss).
