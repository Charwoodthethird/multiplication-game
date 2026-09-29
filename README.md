# NOCLIP: Times Tables

A Minecraft-style, Backrooms-themed multiplication drill for iPad (or any browser).

## Rules
- 4 answer choices. Right answer +1 point, wrong answer −1 (never below 0).
- 10 in a row: +1 bonus. 20 in a row: +2 bonus. Repeats every 20.
- 100 points = 1 coin = the next Backrooms level (new look).
- 5 coins = $1, up to $5 per week (week resets Monday). Extra coins are saved for next week.

## Creature encounters
Every 15–40 minutes of active play (the first one after 4–10 minutes), a Backrooms creature (Smiler, Deathmoth or Partygoer) knocks the question panel away between questions. Tapping 18 times in 5 seconds scares it off for +1 bonus point. Failing costs nothing. Idle time doesn't count toward the timer. The parent screen has a **Test a creature** button.

## How it picks questions
Covers every fact from 0×0 to 12×12 (3×7 and 7×3 count as one fact), in random order.
- **Known** = right on at least 3 of the last 4 tries (or right, quickly, the very first time). A right answer that takes longer than 6 seconds only counts half, so facts he's working out rather than recalling keep coming back.
- Questions are a mix of review (known facts) and learning (facts not yet known). The mix starts at 60/40 and adjusts itself to keep his last 20 answers around 75–85% right, the range where kids stay engaged without getting bored or discouraged. It stays between 40% and 85% review.
- Six not-yet-known facts are in rotation at a time, introduced easiest first (×0, ×1, ×10, ×2, ×5, ×11, ×3, ×4, ×9, ×6, ×12, ×8, ×7). When one becomes known, the next one comes in.
- Review questions favor facts he hasn't seen in a while or missed recently.

## Parent screen
Tap the padlock in the top-right corner. You'll set a 4-digit PIN the first time. From there you can see dollars owed and tap **Mark paid**, view stats and a 12×12 map of known facts, see which facts need practice, change the PIN, or reset everything.
Forgot the PIN? On the iPad, go to Settings → Apps → Safari → Advanced → Website Data and delete this site's data. That resets all progress too.

## Tweaking
The numbers (60/40 split, points per coin, weekly cap, streak bonuses) are in the `CONFIG` block near the top of the script in `index.html`.

## Putting it on the iPad
1. Host on GitHub Pages (repo Settings → Pages → Deploy from branch → `main`, `/ (root)`).
2. On the iPad, open the Pages link in Safari → Share → **Add to Home Screen**.
3. Open it once while online; after that it works offline. Progress is saved on the iPad.
