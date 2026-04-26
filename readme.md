# 🌿 Pheno Hunter
### Cannabis Breeder Simulator · Multi-AI Edition

> Breed the perfect cultivar. Select parents, chase elite phenotypes across generations, and race the market to register a champion. Multi-AI lab partner included — bring your own key.

**Live:** [jkh2.github.io/pheno-hunter-game](https://jkh2.github.io/pheno-hunter-game) · 📖 [Player Manual](MANUAL.md)

---

## What It Is

Pheno Hunter is a reality-inspired cannabis breeding strategy simulator. You're not watering plants — you're making breeder decisions: selecting parents, running phenotype trials, hunting keeper expressions, stabilizing genetics across generations, and reading market demand to time your releases.

The genetic engine models dominant/recessive trait inheritance, phenotype variance, mutation events, and defect risk — based on the real logic experienced breeders use.

---

## Game Loop

1. **Start with real-world foundation cultivars** — Blue Dream, Wedding Cake, Gelato, GG4, Runtz, and more
2. **Run grow seasons** — 5 phases per cycle (Germ → Veg → Flower → Cure → Eval)
3. **Run phenotype trials** — sharpen hidden trait expression before selecting parents
4. **Select two parents and breed** — genetic inheritance produces offspring with trait variation, mutation events, special expressions, and defect risk
5. **Clone keepers** — preserve elite phenotypes before culling
6. **Watch the market** — demand rotates each season (potency vs. bag appeal vs. yield vs. terps)
7. **Sell licensed cuttings** — generate revenue to upgrade your lab
8. **Upgrade the lab** — better selection accuracy, more offspring per cross, sharper trials
9. **Register a Champion** — hit Score 450+ and market value $12,000+ to win

---

## AI Lab Partner

The Lab Partner reads your current game state — best plant data, selected cross, market conditions, and your breeding notes — and gives specific, actionable analysis from the perspective of an expert breeder.

**Supported providers (BYOK):**

| Provider | Model | Key format |
|----------|-------|-----------|
| **Claude** (Anthropic) | claude-sonnet-4-20250514 | `sk-ant-...` |
| **Grok** (xAI) | grok-3-mini | `xai-...` |
| **Gemini** (Google) | gemini-2.0-flash | `AIza...` |
| **Local** | Ollama / LM Studio | endpoint URL |

Keys are never stored — they live only in the browser session. A local fallback analysis runs if no key is entered.

---

## Trait System

| Trait | Affects |
|-------|---------|
| THC (Potency) | Score weight (3.5x), market demand cycles |
| Yield | Score weight (1.05x), revenue base |
| Vigor | Growth speed, event resistance |
| Stability | Defect risk, phenotype consistency |
| Resin | Score weight, extract market value |
| Aroma / Terpenes | Score weight, market demand cycles |
| Bag Appeal | Score weight, market value multiplier |
| Resistance | Mold/pest/heat event damage reduction |
| Flowering Time | Shorter = season efficiency bonus |
| Difficulty | Defect risk modifier |

---

## Scoring

```
Score = THC×3.5 + Yield×1.05 + Vigor×0.45 + Stability×0.65
      + Resin×0.75 + Aroma×0.65 + BagAppeal×0.7 + Resist×0.45
      + FlowerBonus - DifficultyPenalty - DefectPenalty×24
      + KeeperBonus + CloneBonus
```

**Win condition:** Score ≥ 450 AND market value ≥ $12,000

---

## Grow Room

The grow room renders a live canvas view of your current seed bank. Plants visually evolve through all 5 growth phases based on their actual trait values:

- Sativas stretch tall with a natural stem curve and wide canopy spread
- Indicas stay squat and dense with thick stems
- High vigor plants are taller, high yield plants have wider canopy
- High resin plants show trichome sparkle at flower and cure stages
- Purple fade special trait shows as a visible tint on the canopy
- Buds shift from green to amber/gold at cure stage
- Click any plant in the room to select and inspect it

---

## Lab Upgrade Stats

The lab stats panel sits directly below the Upgrade Lab button and shows exactly what each upgrade changes — current values on the left, next level values in gold on the right:

| Stat | What changes |
|------|-------------|
| **Offspring/cross** | More plants produced per breeding round |
| **Trial accuracy** | Lower noise = truer trait expression in pheno trials |
| **Breed cost** | Cost to run a breeding round decreases |
| **Spike chance** | Higher chance of a trait spike in offspring |

The field log entry after each upgrade also spells out the before/after numbers so you always know exactly what you bought.

---

## Random Events

Each completed season has a 32% chance of triggering an event:

- **Mold Outbreak** — damages yield, reduced by resistance
- **Pest Pressure** — hits resin, reduced by resistance
- **Heat Event** — drops vigor scores
- **Compliance Inspection** — flat cash cost
- **Herm Expression** — bag appeal penalty on unstable plants
- **Power Fluctuation** — light stress, minor vigor hit
- **Perfect Conditions** — bonus cash harvest
- **Bumper Terp Season** — aroma spike + bonus revenue

---

## Strain Browser

Pheno Hunter includes a live strain browser powered by the **Kushy Cannabis Dataset** (MIT License, hosted on GitHub).

- **9,482 real strains** loaded directly from the dataset on demand
- Search by name or breeder
- Filter by type (Indica / Sativa / Hybrid), effect, and flavor
- Select any strain to preview its projected game stats before importing
- **Import as Foundation Cultivar** — adds the strain to your current seed bank
- **Import + Reset Seed Bank** — starts fresh with your chosen strain as the primary cultivar

Game stats (THC, Yield, Vigor, Stability, Resin, Aroma, Bag Appeal, Resistance) are algorithmically derived from the real strain data — type sets the baseline, effects and flavor profiles apply stat biases, and light random variance is added so no two imports are identical.

Data source: [github.com/kushyapp/cannabis-dataset](https://github.com/kushyapp/cannabis-dataset) · MIT License

---

## Deployment

Single `index.html` — no build step, no dependencies, no framework.

**GitHub Pages:**
1. Fork or clone this repo
2. Go to Settings → Pages → Source: main branch / root
3. Done — live at `yourusername.github.io/pheno-hunter-game`

---

## Tech

- Vanilla JS, HTML5, CSS3, Canvas API
- Google Fonts: Share Tech Mono + Rajdhani
- No npm, no build, no framework
- localStorage save/load
- Multi-provider AI via direct fetch (Claude, Grok, Gemini, local Ollama)
- Live grow room rendered in HTML5 Canvas

---

## Credits

Built by **James Keith Harwood II** · [Sentinel AI Systems](https://jameskeithharwood.com)  
AI development partner: **Claude Sentinel** (Anthropic)

Cultivar data is reality-inspired game abstraction — not grow instructions.  
All gameplay takes place in a fictional simulation context.

---

*"The endgame is an AI-assisted lab partner that helps analyze your breeding program."*
