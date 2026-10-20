# Dough Batch Planner

A one-page calculator for planning pizza dough batches.

Enter the trays needed for each size and it splits them into batches. Each batch is one 1,216 oz dough ball (8 trays × 8 larges × 19 oz).

| Size | Dough ball | Per tray |
|------|-----------:|---------:|
| P (Pizzoli) | 5 oz | 12 |
| S (Small) | 10 oz | 10 |
| M (Medium) | 14 oz | 9 |
| L (Large) | 19 oz | 8 |
| XL | 25 oz | 6 |

## How it plans

1. Uses the fewest batches possible.
2. Keeps as many batches single-size as it can.
3. If an order is just over a batch line, saves a whole batch by letting one or two sizes come up a few dough balls short (always less than a tray). Tap the tip to use the extra batch instead.
4. Shares the leftover dough across sizes ("Spread"), or puts it all into the size you pick.

## Reading the chart

- **#**: trays to cut
- **R**: the rest of the dough in that batch goes to this size
- **A**: the whole batch goes to this size

Tap a batch number to check it off once it's made.

## Changing the numbers

Dough weights and tray counts are in the `SIZES` list near the top of the script in `index.html`. The batch size is `CAP`.
