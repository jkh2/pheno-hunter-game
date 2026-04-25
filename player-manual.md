# 🌿 Pheno Hunter — Player's Manual

> You're not a gardener. You're a breeder. Your job is to hunt elite genetics, stabilize a champion line, and release a cultivar worth $750,000 to the market.

---

## The Goal

Breed a plant that hits **Score 450 or higher** AND has a **Market Value of $750,000+**.

When you hit both thresholds, click **Register Champion** and you win.

It takes several generations and smart decision-making to get there. Don't expect to win on your first run.

---

## The Interface

The screen is divided into two columns.

**Left column** — your grow room and seed bank. This is where you see your plants, the market, and your field log.

**Right column** — your controls. Best plant display, lab actions, and the AI Lab Partner.

---

## The Stats Bar (Top of Screen)

| Stat | What It Means |
|------|--------------|
| **Season** | How many grow cycles you've completed |
| **Cash** | Your available funds — don't let this hit zero |
| **Best Score** | The score of your top-ranked plant right now |
| **Generation** | What breeding generation you're in (F0 = foundation stock, F1 = first cross, etc.) |
| **Win Goal** | Fixed at 450 points — your target |

---

## The Grow Cycle Bar

Every grow season moves through **5 phases** in order:

```
GERM → VEG → FLOWER → CURE → EVAL
```

Each time you click **Run Grow Season**, you advance one phase and spend cash. When you complete all 5 phases (EVAL), the season ends, your cash resets the market, and a random event may fire.

The little dots across the bar show which phase you're in. Green = done, blinking = current, dark = ahead.

**Important:** You cannot skip phases. Each one costs money. Plan your cash accordingly.

---

## The Seed Bank (Left Tab)

This is your plant list, ranked best to worst by score.

Each plant card shows:
- **Name** and generation (F0, F1, F2...)
- **Terpene profile** and **flowering time** in days
- **Green badges** — special traits (fuel nose, dense stacking, greasy resin, etc.)
- **Red badges** — defects (herm tendency, mold sensitivity, weak stems, etc.)
- **Blue badges** — clone saved or keeper status
- **Trait bars** — THC, Yield, Resin, Bag Appeal
- **Score** (top right corner of card)
- **Market Value** (bottom of card)

**To select a parent plant:** Click it. A green border appears. Click a second plant to select your breeding pair. The hint text at the bottom confirms your selection.

---

## The Market Tab

Shows what the market is paying a premium for **this season**. Rotates every season.

- **★ Primary demand** — highest bonus, the trait to align with
- **◆ Secondary demand** — moderate bonus
- Everything else — base value only

Check this before selling cuttings. A plant with high Bag Appeal is worth far more in a Bag Appeal season than a Potency season.

---

## The Field Log Tab

A running record of everything that's happened — breeds, sales, events, upgrades. Good for tracking your progress and catching patterns.

---

## Lab Actions (Right Column)

These are your main controls. Here's what each one does and when to use it.

---

### 🟢 Run Grow Season
**Cost:** Increases each season (~$850 early, more later)

Advances your grow cycle one phase. Do this 5 times to complete a full season. Each completed season:
- Rotates the market
- May trigger a random event (mold, pests, heat, inspections, or a bonus)
- Costs cash you need to budget for

**Use when:** You're ready to push forward. Don't run seasons if you're broke — you need cash to breed and trial.

---

### 🔬 Pheno Trial
**Cost:** $220

Runs a more precise expression test on all your plants. Hidden genetic potential becomes more visible — trait bars shift to reflect truer values. Higher lab levels make trials more accurate.

**Use when:** You've just bred a new generation and want to see which offspring are actually worth keeping before you breed again. Always trial before selecting new parents.

---

### 🧬 Breed Parents
**Cost:** ~$445 (decreases as you upgrade the lab)

Takes your two selected parents and produces offspring. The number of offspring increases with your lab level. After breeding:
- New plants appear ranked by score
- Clone-saved and keeper plants are protected from culling
- Your generation counter advances (F1, F2, F3...)

**Use when:** You have two parents selected and have run a pheno trial. Don't breed blind — trial first.

---

### 💾 Clone Best
**Cost:** $160

Saves a clone of your current top-ranked plant. Cloned plants survive future culling when you breed — they won't get cut from the gene pool no matter what.

**Use when:** You find a phenotype with an exceptional trait combination you don't want to lose. Clone before you breed, not after.

---

### 📋 Toggle Keeper
**Cost:** Free

Marks your top plant as a keeper. Keeper plants also survive culling. Gives a small score bonus.

**Use when:** A plant isn't your absolute best but has traits you want to preserve for future crosses — high stability, clean defect profile, good resistance.

---

### 💰 Sell Licensed Cuttings
**Cost:** Free — earns money

Sells cuttings from your top-ranked plant at current market value. This is your primary income source. Market value is calculated from score, generation scarcity, defect drag, and current market demand bonus.

**Use when:** Your best plant aligns with the current market's primary demand trait. Don't sell into a bad market if you can wait a season.

---

### ⬆️ Upgrade Lab
**Cost:** $1,450 → increases each level

Upgrades your lab to the next level. Each upgrade gives you:
- More offspring per breeding round
- More accurate pheno trials (less hidden variance)
- Slightly higher mutation discovery chance (rare spike events)
- Cheaper breeding costs

**Use when:** You've built up cash and are ready to push into deeper generations. Lab Level 2 is a big jump — prioritize it early.

---

### 🏆 Register Champion
**Cost:** Free — triggers win check

Checks if your top plant meets the win conditions (Score 450+ and Market Value $750k+). If it does, you win. If not, it tells you how far off you are.

**Use when:** Your best score is approaching 400+ and your market value is climbing. Check often — you might be closer than you think.

---

## The AI Lab Partner

The Lab Partner reads your current game state and gives you specific breeding recommendations.

**To use it:**
1. Pick a provider tab — **Claude**, **Grok**, **Gemini**, or **Local**
2. Enter your API key for that provider
3. Optionally type notes in the breeding notes box (goals, observations, what you're chasing)
4. Click **Ask Lab Partner**

The partner reads your best plant's full trait profile, your selected cross if any, the current market demand, and your notes — then gives you 2-3 actionable recommendations.

If you don't have an API key, it still runs a local fallback analysis. Less detailed, but useful.

**Keys are never stored.** They exist only in your browser session and disappear when you close the tab.

---

## Random Events

At the end of each completed season there's a ~32% chance of a random event. Events can hurt or help.

| Event | Effect |
|-------|--------|
| **Mold Outbreak** | Yield damage — reduced by Resistance stat |
| **Pest Pressure** | Resin damage — reduced by Resistance stat |
| **Compliance Check** | Flat $150 cash cost |
| **Heat Event** | Vigor drops across all plants |
| **Herm Expression** | Bag Appeal penalty on plants with herm tendency defect |
| **Power Fluctuation** | Minor vigor stress, small cash cost |
| **Perfect Conditions** | +$600 cash bonus |
| **Bumper Terp Season** | Aroma spike + $200 bonus |

High Resistance and low Difficulty scores protect you from event damage. Unstable plants with herm tendency defects are especially vulnerable.

---

## Traits Explained

| Trait | What It Does |
|-------|-------------|
| **THC (Potency)** | Highest score weight (3.5x). Market demand cycles include Potency seasons. |
| **Yield** | Score weight 1.05x. Base revenue driver. |
| **Vigor** | Affects grow speed and event resistance. Lower score weight but important for survivability. |
| **Stability** | Reduces defect risk in offspring. Low stability = more defects in future generations. |
| **Resin** | Score weight 0.75x. Drives extract market value. |
| **Aroma / Terps** | Score weight 0.65x. Cycles as a primary market demand trait. |
| **Bag Appeal** | Score weight 0.7x AND multiplies market value. One of the most important commercial traits. |
| **Resistance** | Reduces damage from mold, pest, and heat events. |
| **Flowering Time** | Shorter = score bonus. Shown in days on each card. |
| **Difficulty** | Higher difficulty = higher defect risk. Watch this in your parents. |

---

## Defects and Special Traits

**Defects** (red badges) penalize your score by 24 points each and drag market value down. They can appear in offspring from unstable crosses. The most dangerous is **herm tendency** — it triggers bonus penalties during Herm Expression events.

**Special traits** (green badges) are flavor expressions that appear on every plant. They don't directly affect score but reflect the character of the phenotype. Future versions will add trait-specific bonuses.

---

## Basic Strategy Guide

**Early game (F0–F1):**
- Don't breed immediately. Run a pheno trial first to see true trait values.
- Sell cuttings from your best F0 plant to build cash.
- Upgrade the lab to Level 2 before going deep into generations.
- Look for parents with high stability — it protects your offspring from defects.

**Mid game (F2–F4):**
- Clone any plant scoring above 300 before you breed.
- Watch the market — time your cuttings sales to primary demand seasons.
- Run pheno trials every generation before selecting new parents.
- Avoid breeding two defect-heavy parents — defects compound.

**Late game (F5+):**
- Your best plants should be scoring 350–420. You need one more push.
- Look for the spike event in breeding — occasionally one trait jumps hard. That's your champion candidate.
- Clone it immediately. Sell cuttings in the right market season to push market value past $750k.
- Register the champion.

---

## Save and Load

**Save** — stores your full game state to your browser's local storage. Use it before closing the tab.

**Load** — restores your last save. Only one save slot exists per browser.

**New Game** — starts fresh. Your save is not overwritten until you save again.

---

## Scoring Formula

```
Score = THC×3.5 + Yield×1.05 + Vigor×0.45 + Stability×0.65
      + Resin×0.75 + Aroma×0.65 + BagAppeal×0.70 + Resist×0.45
      + FlowerBonus (shorter = better, max ~20pts)
      - DifficultyPenalty×0.28
      - DefectPenalty×24 per defect
      + KeeperBonus (20pts)
      + CloneBonus (12pts)
```

Maximum theoretical score: ~520. Win threshold: 450.

---

*Pheno Hunter v1.0 · Sentinel AI Systems · [jkh2.github.io/pheno-hunter-game](https://jkh2.github.io/pheno-hunter-game)*
