Run in order (edit the CSV path inside screen.py to your Scopus export):
 1. screen.py   - load export, first-pass rules (superseded; builds scr.pkl)
 2. screen2.py  - second-pass rules (superseded; builds scr2.pkl)
 3. screen3.py  - FINAL screening rules (IC1/IC2/off-topic); builds scr3.pkl; draws validation sample (seed 7)
 4. analyze.py  - dedupe, bibliometrics, AI-family/task/validation coding, keyword clusters -> results.json, coded_included.csv
 5. figs.py     - Fig. 1 (PRISMA), Fig. 2, Fig. 3
Validation files: validation.csv (development sample, kappa 0.42), validation2.csv (fresh sample, kappa 0.55).
Requires: pandas, matplotlib, networkx, scikit-learn.
