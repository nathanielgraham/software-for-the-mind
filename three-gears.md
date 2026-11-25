# Three Gears for Blitz (and Beyond)

A practical system for choosing how much model to build on any given move. The goal is maximum return per second of clock: a tiny complete picture beats a larger incomplete one.

## Why a complete model (and why three gears)

In slower chess the natural loop is: build a full model → generate candidates → analyze them. Under a blitz or rapid clock that loop is usually too expensive. Spending it on every move produces a foggy picture and a flag.

A complete model, even a tiny one, is better than a larger incomplete one because it lets you move with a coherent reason instead of residual doubt. The three gears force the size of the model to match the time you actually have:

- Gear 1 keeps you alive when something can die immediately.
- Gear 2 gives you a full (if minimal) picture on ordinary moves.
- Gear 3 adds only the extra filters that change the evaluation, then stops.

You never try to see everything. You see enough to act, inside a hard time box. The same structure works for most players and most time controls; only the size of the boxes and the number of deeper sits change.

## The Three Gears

| Gear | Name | Blitz box | Longer box | What you do | Stop & move when |
|------|------|-----------|------------|-------------|------------------|
| 1 | CCT | 1–2s | 3–5s | Checks, captures, crude next-move threats only | Something can die this move |
| 2 | Tiny model | ~3s | 10–15s | CCT clean + four questions (below) | You have a candidate |
| 3 | Working model | 6–15s | 30–60s | Gear 2 + hanging pieces, weak/important squares, one clear motif. Then compare at most two candidates. | Two concrete candidates exist, or the time box ends |

Default is Gear 1, then Gear 2. Gear 3 is the exception.

### Gear 1 — CCT

- Checks (theirs, then yours)
- Captures (hangs, recaptures, material)
- Threats = next-move forced pain you can point at in one glance (piece taken, mate you see, promotion, check-and-piece)

If you cannot point at the square and the piece immediately, it is not a CCT threat.  
Use this for the first 8–10 moves of a prepared opening and any time a clock checkpoint has already been missed.

### Gear 2 — Tiny model (~3s in blitz)

After CCT is clean, answer four questions and play the move they imply:

1. King safety — one phrase (fine / loose / both airy).
2. The one break or open file the position is about.
3. Worst-placed piece — yours, then theirs.
4. Play the obvious improving move that sentence implies.

If the four questions produce zero candidates inside the time box, play a developing or improving move. Do not open a longer sit because the model felt incomplete.

### Gear 3 — Working model

Gear 2 plus:
- Hanging pieces (yours and theirs)
- Weak or important squares
- One clear tactical motif (pin, fork, discovery, back-rank, etc.)

Then compare at most two concrete candidates and pick one.  
If after the time box you still do not have two candidates, drop back to Gear 2 and move.

## Hard rules

- Miss a clock checkpoint → drop to Gear 1 for the rest of the game.
- Gear 3 has a hard per-game quota (example: one or two sits in 5+0; fewer in 3+0). Once the quota is gone, the cap drops.
- Prepared opening moves 1–8/10: play the line. Do not rebuild a model.
- Zero candidates inside a gear’s time box → play a developing or improving move. Do not escalate.

## Optional pattern triggers

After Gear 2 is clean, glance at one or two of these only if the board literally shows the pattern. They are cheap insurance, not a checklist. Never let them override the time box or the “zero candidates → move” rule.

- Opponent’s high-value pieces on the same color as your knight → check for forks.
- Open file + rook still on the back rank → check back-rank or invasion.
- King and queen aligned with your bishop or rook → check the pin or discovery.
- Clear outpost or weak square created by the pawn structure → see if a piece can sit there in one move.

Cap yourself at two triggers. If you start running through every heuristic you know, you have left the system.

## Clock checkpoints (example for 5+0)

| Move | Minimum clock |
|------|----------------|
| 15 | 3:30 |
| 25 | 2:00 |
| 35 | 1:00 |
| 45 | 0:30 |

Miss one → Gear 1 only to the end. Adjust the numbers for other controls; the principle stays the same.

## Why this is high-ROI

- Gear 1 catches the things that lose games immediately.
- Gear 2 forces a complete (if tiny) picture instead of a foggy one.
- Gear 3 adds only the practical middlegame filters that actually change the evaluation, then stops.
- Longer variations, minor piece improvements, and abstract plans are left for post-game review or for the rare position where Gear 3 still leaves the game on a knife-edge and the clock still allows it.

The same three gears work for most players and most time controls. Only the size of the boxes and the number of Gear 3 sits change.
