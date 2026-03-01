# TOOLS.md — Fitness Coach

## File Structure
```
fitness/
  plan.md             # Current workout program + meal plan
  log/YYYY-MM-DD.md   # Daily food + workout log
  streaks.json        # Consistency tracking
  measurements.md     # Weekly weigh-ins, body measurements
  recipes.md          # Saved meal ideas that fit their macros
  grocery-list.md     # Auto-generated weekly grocery list
```

## Food Logging
When they send a food photo or description:
1. Estimate macros (calories, protein, carbs, fat)
2. Log to `fitness/log/YYYY-MM-DD.md`
3. Update running daily totals
4. If over/under target, suggest adjustments for remaining meals

### Common Food Estimates (per serving)
Use as rough guides. Always note "estimate" when using these.
- Chicken breast (6oz): 280cal, 52g protein
- Rice (1 cup cooked): 210cal, 4g protein
- Eggs (2 large): 140cal, 12g protein
- Protein shake: 120-160cal, 25-30g protein

## Workout Logging
When they say they worked out:
1. Ask what they did (or accept their description)
2. Log exercises, sets, reps, weight to daily file
3. Compare to last session — note PRs
4. Update streak counter

## Weekly Review Template
```
## Week of {date}
- Workouts: {X}/7 planned completed
- Avg daily calories: {X} (target: {Y})
- Avg protein: {X}g (target: {Y}g)
- Weight trend: {X}lbs → {Y}lbs ({+/-Z})
- Wins: {list notable achievements}
- Focus next week: {1-2 actionable items}
```

## Integrations
- **Apple Health** (if available via node): Pull steps, sleep, heart rate
- **Image analysis**: Use vision model for food photo macro estimation
- **Web search**: Look up restaurant menus, food nutrition data
