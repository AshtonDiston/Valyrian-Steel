# Valyrian Steel – CK3 AGOT Submod

A submod for the **A Game of Thrones (AGOT)** mod for **Crusader Kings 3**. It adds new decisions, artifacts, and mechanics centred around the ancient civilization of Old Valyria.

---

## What This Submod Adds

### Decisions

| Decision | Cost | Requirement |
|---|---|---|
| Fund an Expedition to Old Valyria | 500 Gold | Landed, not at war, not a Wildling culture |
| Hire Master Blacksmith | 300 Gold | Landed ruler, no Court Smith already employed |
| Research Dragonlore | Free | Must possess the Valyrian Book and know the Valyrian language |
| Enchant Dragon Horn | 500 Piety | Must own an unenchanted Dragon Horn; must have Dragonblood heritage (based on game rules) |
| Un-Enchant Dragon Horn | 100 Piety + 100 Prestige | Must own an enchanted Dragon Horn |

### Artifacts

All of the following artifacts can be obtained through the **Fund Expedition** decision (or its focused variants):

- **Valyrian Steel Sword** – A powerful weapon recovered from the ruins of Old Valyria. Grants high Prowess bonuses.
- **Valyrian Steel Axe** – Rare Valyrian axe. Grants Prowess bonuses.
- **Valyrian Steel Mace** – Rare Valyrian mace. Grants Prowess bonuses.
- **Valyrian Steel Spear** – Rare Valyrian spear. Grants Prowess bonuses.
- **Valyrian Steel Dagger** – Rare Valyrian dagger. Grants Prowess bonuses.
- **Valyrian Steel Halberd** – Rare Valyrian halberd. Grants Prowess bonuses.
- **Dragon Egg** – An unhatched dragon egg from Old Valyria. A reminder of Valyrian power; may one day hatch.
- **Dragon Horn** – An ancient artifact used by Valyrian Dragonlords to command dragons. Can be enchanted (with Dragonblood heritage) to increase your dragon-bonding scheme chance. *Warning: while enchanted, the horn slowly drains your health.*
- **Dragon Whip** – A whip crafted from rare metals and dragon leather, used to command dragons. Boosts dragon-bonding scheme success chance for those with Dragonblood heritage.
- **Valyrian Book** – An ancient tome written in Old Valyrian. Enables the **Research Dragonlore** decision (requires knowing the Valyrian language), and boosts dragon-bonding scheme success for those with Dragonblood heritage.
- **Glass Candle** – A mystical candle from Old Valyria. Also returns some gold to partially offset expedition costs.
- **Valyrian Steel Goblet** – A finely crafted Valyrian Steel cup. Can be **reforged** into a greater weapon by a Court Smith.

### Other Mechanics

- **Hire Master Blacksmith decision** – Appoints a master smith from Qohor as your Court Smith, enabling you to reforge Valyrian Steel artifacts (e.g. the VS Goblet into a weapon).
- **Research Dragonlore decision** – Requires the Valyrian Book and knowledge of the Valyrian language. Unlocks ancient dragon-bonding knowledge.
- **Bond with Dragon scheme** – A Diplomacy-based scheme to bond with and tame a wild dragon. Success chance is boosted by Dragonblood heritage, the Dragon Horn (enchanted), Dragon Whip, and Valyrian Book.

---

## Fund Expedition to Old Valyria – Outcome Chances

The decision costs **2500 Gold** and has a **10-year cooldown** (the cooldown is removed if the expedition leader dies without returning an artifact).

### Step 1 – Choosing your explorer

You are presented with three candidates from your court or vassals. You can choose any of the three, or cancel the expedition entirely.

### Step 2 – Focusing the expedition (optional extra cost)

After choosing your explorer, you may pay additional gold to focus the search:

| Focus | Extra Cost | Guaranteed Artifact |
|---|---|---|
| Find a Dragon Egg | +750 Gold | Dragon Egg (100%) |
| Find a Valyrian Steel Weapon | +750 Gold | Valyrian Steel weapon (100%) |
| Find a Trinket | +250 Gold | One random trinket (equal chance) |
| Find Anything | +0 Gold | Random artifact (see odds below) |

### Step 3 – Expedition outcome

After roughly 30–60 days, one of three outcomes occurs:

| Outcome | Weight | Probability (epidemics on) | Probability (epidemics off) |
|---|---|---|---|
| **Leader dies / does not return** – No artifact; expedition cooldown is refunded | 8 | 80% | ~88.9% |
| **Leader returns extremely sick** – Brings back an artifact but is gravely ill (disease) | 1 | 10% | N/A (disabled) |
| **Successful return** – Leader returns unharmed with an artifact | 1 | 10% | ~11.1% |

> **Note:** The "sick return" outcome only fires when the *epidemic_frequency_disabled* game rule is **not** active. When epidemics are disabled (*epidemic_frequency_disabled* is active), that outcome is skipped and the total weight is 9 (not 10).
>
> In **2 out of 3** outcomes (sick and successful) the expedition leader brings back an artifact. Only if the leader dies do you receive nothing.

**Overall chance of receiving an artifact:**
- Epidemics **enabled**: 2 ÷ 10 = **20%**
- Epidemics **disabled**: 1 ÷ 9 ≈ **11.1%**

### Step 4 – Artifact rolled (when no focus is chosen)

When you choose "Find Anything" (no additional cost), the artifact is determined by a weighted random roll:

| Artifact | Weight | Probability of this artifact (given artifact returned) |
|---|---|---|
| Valyrian Steel weapon | 33 | ~34.4% |
| Dragon Egg | 33 | ~34.4% |
| Rare Trinket *(Dragon Horn, Dragon Whip, or Valyrian Book – equal chance among the three)* | 15 | ~15.6% total (~5.2% each) |
| Misc Artifact *(Glass Candle or Valyrian Steel Goblet – equal chance between the two)* | 15 | ~15.6% total (~7.8% each) |

*Total weight: 96*

When you choose "Find a Trinket" (+100 Gold), the trinket pool is expanded and each of the five trinkets (Dragon Horn, Dragon Whip, Valyrian Book, Glass Candle, Valyrian Steel Goblet) has an **equal 20% chance**.

### Combined odds (epidemics enabled, no focus)

| Result | Combined chance |
|---|---|
| Get a Valyrian Steel weapon | 20% × 34.4% ≈ **6.9%** |
| Get a Dragon Egg | 20% × 34.4% ≈ **6.9%** |
| Get a Dragon Horn | 20% × 5.2% ≈ **1.0%** |
| Get a Dragon Whip | 20% × 5.2% ≈ **1.0%** |
| Get a Valyrian Book | 20% × 5.2% ≈ **1.0%** |
| Get a Glass Candle | 20% × 7.8% ≈ **1.6%** |
| Get a Valyrian Steel Goblet | 20% × 7.8% ≈ **1.6%** |
| Expedition leader dies, no artifact | **80%** |