# Carcassonne Lake Expansion — Full Rules

## Overview

A new edge type for Carcassonne featuring lakes that score like cities but with a fishing twist.

**Contents:** [Setup](#setup) · [Core Rules](#core-rules) · [Fish Icons](#fish-icons) · [Treasure Island](#special-tile-treasure-island) · [Scoring Examples](#scoring-examples) · [Tile Set](#tile-set-25-tiles) · [Interactions](#interactions) · [Edge Cases](#edge-cases) · [Strategy Tips](#strategy-tips) · [Compatibility](#compatibility) · [Design Notes](#design-notes)

---

## Setup

1. Shuffle the 25 lake tiles into the base game tile stack.
2. Each player takes **2 fishermen** in their color, in addition to their normal meeples. (Provisional: the final count will be set by playtesting, see [development plan §2.4](development-plan.md#24-design-fisherman-meeple).)
3. Play as normal. All base game rules apply unless these rules say otherwise.

---

## Core Rules

### Lake Edges

Lake edges must connect to other lake edges, just like city walls must connect to city walls. A lake is **complete** when fully enclosed with no open lake edges.

### Meeple Placement

Place a **Fisherman** on a lake to claim it. The fisherman works exactly like a knight in a city:

- You may place a fisherman only on the lake segment of the tile you just placed, and only if that lake has no fisherman on it yet
- If two lakes merge, the player(s) with the most fishermen score the lake
- Ties result in all tied players scoring full points
- After a lake is scored, all fishermen on it return to their owners

### Scoring

| Condition | Points |
|-----------|--------|
| Completed lake | 2 points per tile + 1 point per fish icon |
| Incomplete lake at game end | 0 points |

This creates real tension—lakes are worthless if you can't close them, so there's risk in starting large ones and opportunity to sabotage opponents.

### Single-Tile Lakes

Every lake tile has at least one open lake edge, so no single tile is ever a complete lake. The smallest possible lake is two Caps placed lake-edge to lake-edge. You may place a fisherman on a newly started one-tile lake, but it scores nothing unless the lake is later completed.

---

## Fish Icons

Some lake tiles have fish icons (1-3 fish) printed on them. Fish add bonus points when the lake is completed.

**Distribution principle:** Riskier tiles have more fish.

- Caps (easy to close): 0 fish
- Corners/Straights: 0-1 fish
- T-Shapes: 1-2 fish
- Open Water: 2-3 fish
- Treasure Islands: 1 fish (the doubling is their main reward)

---

## Special Tile: Treasure Island

**2 tiles in the set** feature a small island in the center of the lake.

**Effect:** When the lake is completed, **double the total score**.

### Stacking Rule

Only one doubling applies. If both Treasure Islands end up in the same lake, the second one just counts as a normal tile (no quadrupling).

### Treasure Island Design

Treasure Island tiles have 3-4 lake edges, making them committal. You can't easily close a lake containing a Treasure Island—you need to build big.

---

## Scoring Examples

### Example 1: Small Lake
- 3 tiles, 1 fish (Cap + Straight 1 + Cap)
- Score: (3 × 2) + 1 = **7 points**

### Example 2: Medium Lake
- 5 tiles, 4 fish (Corners 1, 2 and 4 plus T-Shape 3 in a 2×2 ring; the T-Shape's third lake edge is closed with a Cap)
- Score: (5 × 2) + 4 = **14 points**

### Example 3: Large Lake
- 8 tiles, 9 fish
- Score: (8 × 2) + 9 = **25 points**

### Example 4: Large Lake with Treasure Island
- 8 tiles, 9 fish, 1 Treasure Island
- Base score: (8 × 2) + 9 = 25
- Doubled: **50 points**

### Example 5: Incomplete Lake
- Any size, any fish
- Score: **0 points**

---

## Tile Set (25 tiles)

### Caps — 1 lake edge (8 tiles)

| Tile | Top | Right | Bottom | Left | Fish |
|------|-----|-------|--------|------|------|
| Cap 1 | Field | Field | Lake | Field | 0 |
| Cap 2 | Field | Field | Lake | Road | 0 |
| Cap 3 | Field | Road | Lake | Road | 0 |
| Cap 4 | Road | Field | Lake | Field | 0 |
| Cap 5 | City | Field | Lake | Field | 0 |
| Cap 6 | City | Field | Lake | City | 0 |
| Cap 7 | Field | City | Lake | Road | 0 |
| Cap 8 | City | City | Lake | Field | 0 |

### Corners — 2 adjacent lake edges (6 tiles)

| Tile | Top | Right | Bottom | Left | Fish |
|------|-----|-------|--------|------|------|
| Corner 1 | Field | Lake | Lake | Field | 0 |
| Corner 2 | Field | Lake | Lake | Road | 1 |
| Corner 3 | Road | Lake | Lake | Road | 0 |
| Corner 4 | City | Lake | Lake | Field | 1 |
| Corner 5 | City | Lake | Lake | City | 1 |
| Corner 6 | City | Lake | Lake | Road | 1 |

### Straights — 2 opposite lake edges (4 tiles)

| Tile | Top | Right | Bottom | Left | Fish |
|------|-----|-------|--------|------|------|
| Straight 1 | Field | Lake | Field | Lake | 1 |
| Straight 2 | Road | Lake | Field | Lake | 1 |
| Straight 3 | Road | Lake | Road | Lake | 1 |
| Straight 4 | City | Lake | Field | Lake | 1 |

### T-Shapes — 3 lake edges (3 tiles)

| Tile | Top | Right | Bottom | Left | Fish |
|------|-----|-------|--------|------|------|
| T-Shape 1 | Field | Lake | Lake | Lake | 2 |
| T-Shape 2 | Road | Lake | Lake | Lake | 1 |
| T-Shape 3 | City | Lake | Lake | Lake | 2 |

### Open Water — 4 lake edges (2 tiles)

| Tile | Top | Right | Bottom | Left | Fish |
|------|-----|-------|--------|------|------|
| Open Water 1 | Lake | Lake | Lake | Lake | 2 |
| Open Water 2 | Lake | Lake | Lake | Lake | 3 |

### Treasure Island — 3-4 lake edges (2 tiles)

| Tile | Top | Right | Bottom | Left | Fish | Special |
|------|-----|-------|--------|------|------|---------|
| Treasure 1 | Field | Lake | Lake | Lake | 1 | 2× score |
| Treasure 2 | Lake | Lake | Lake | Lake | 1 | 2× score |

---

## Total Fish Distribution

| Tile Type | Tiles | Total Fish |
|-----------|-------|------------|
| Caps | 8 | 0 |
| Corners | 6 | 4 |
| Straights | 4 | 4 |
| T-Shapes | 3 | 5 |
| Open Water | 2 | 5 |
| Treasure Island | 2 | 2 |
| **Total** | **25** | **20** |

---

## Interactions

### Lakes and Fields

Lakes interrupt fields, similar to rivers. A field on one side of a lake is separate from a field on the other side.

### Lakes and Roads

Roads can end at lakes (fishing villages) or pass alongside them. Roads on lake tiles work normally.

### Merging Lakes

When placing a tile that connects two separate lakes:

1. The lakes merge into one
2. Count all fishermen from both original lakes
3. Player(s) with the most fishermen will score when complete
4. If a lake contains multiple Treasure Islands, only one doubling applies

---

## Edge Cases

### Uncompletable Lake
If the remaining tile stack makes it impossible to close a lake (e.g., no caps remain), it scores zero at game end. Players must judge this risk during play—there is no compensation for an impossible-to-complete lake.

### One Tile Touching Two Lakes
All lake edges on a tile belong to the same body of water. So a tile can never complete two *separate* lakes. If its lake edges touch two or more existing lakes, those lakes merge into one (see [Merging Lakes](#merging-lakes)). That merged lake is complete only if it has no open lake edges left. For example, a Straight placed between two lakes joins them into a single lake.

### Cross-Expansion Interactions
When lake edges would need to interact with a non-lake feature from another expansion (e.g., a bridge from Bridges, Castles & Bazaars crossing over a lake edge), treat the lake edge as impassable terrain—the bridge does not connect or close the lake.

---

## Strategy Tips

1. **Small lakes are safe but low-scoring** — Easy to close but few fish
2. **Large lakes are risky** — High potential but opponents can sabotage
3. **Treasure Islands are targets** — Expect interference if you start one
4. **Caps are precious** — Save them for closing, not starting
5. **Watch for sabotage** — An incomplete lake scores zero; use this against opponents

---

## Compatibility

This expansion is designed to work with:

- **Carcassonne base game** (required)
- **Inns & Cathedrals** — Lakes work as a third competitive structure alongside cities and roads. An "Inn on a Lake" variant is a natural extension: mark specific lake-edge tiles with an inn token that doubles the per-tile value (or zeroes it if incomplete), mirroring the Inn on a Road rule.
- **Traders & Builders** — Fish icons are independent of trade goods and do not count as Traders & Builders commodities. The Builder cannot be placed on a lake.
- **The River** — Lake tiles may be placed alongside river tiles; they are independent terrain types.
- **Other expansions** — No known conflicts, but lakes have not been tested with Abbey & Mayor or the Princess & Dragon. Treat lake edges as equivalent to city walls for any expansion rule that references "enclosed feature."

---

## Design Notes

- Caps have no fish to discourage tiny safe lakes
- Fish increase with commitment (more lake edges = more risk = more fish)
- Treasure Islands require 3-4 lake edges, forcing ambitious play
- Enough caps and corners to close lakes reliably
- The 0-point incomplete rule creates tension and interaction
