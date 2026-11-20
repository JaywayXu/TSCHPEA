# T-ITS TSCHPEA

**A Two Stage Cooperative Heterogeneous Parallel Evolutionary Algorithm for Large-Scale Bi-objective Vehicle Routing Problem With Time Windows Under Fleet-Size Preferences**

Zhiwei Xu, Pingshan Wu, Kai Zhang, Quanyu Zhang, Yiran Huang, Juanjuan He, Miqing Li, and Javier Del Ser. Corresponding author: Kai Zhang.

## Highlights

- TSCHPEA first reduces fleet size, then minimizes travel distance at the smallest fleet size found.
- Parallel populations use different initial routes, constraint penalties, and search neighborhoods to explore alternative customer assignments.
- The populations share solutions with low constraint violation during fleet reduction and feasible elite solutions during distance refinement.

## Usage

Use Python 3.12 and a 1,000-customer Gehring–Homberger instance in text format.

```bash
python -m pip install pyvrp==0.12.2 numpy==2.3.5
python TSCHPEA.py INSTANCE.txt --target-fs TARGET
```

Replace `INSTANCE.txt` with the input file and `TARGET` with the Stage 1 fleet-size target. The program prints the fleet size and total travel distance.

## Copyright

Copyright © 2026 the TSCHPEA contributors. The source includes the copyright and license notice for the portions derived from PyVRP.
