# 🏎️ F1 Abu Dhabi 2021 — Race Analysis

Analysis of the 2021 Abu Dhabi Grand Prix — the race that decided the
Formula 1 World Championship between Lewis Hamilton and Max Verstappen.

  Project Overview
Using the FastF1 Python library, this project analyzes real telemetry
and timing data from all 58 laps of the race, culminating in a
physics-level breakdown of the exact lap the championship changed hands.

  Key Findings
- Verstappen's fresh Soft tyres gave him a 0.578s per lap pace advantage
  over Hamilton's degraded Hard tyres in the final stint
- Over 5 laps that compounded to a ~2.89s structural pace deficit
  for Hamilton — making the overtake physically inevitable
- Hamilton led for 57 of 58 laps, building an 11-second gap before
  the Latifi safety car erased it entirely on lap 53
- Lap 58 telemetry shows Verstappen carrying higher corner speed,
  getting on throttle earlier, and braking later — all direct
  consequences of fresh tyre grip

 Project Structure
- Phase 0 — Race gap & position timeline (macro story)
- Phase 1 — Full 58-lap race pace analysis
- Phase 2 — Tyre strategy & degradation modeling by compound
- Phase 2B — Performance delta calculation (quantified pace gap)
- Phase 3 — Lap 58 telemetry dashboard (speed, throttle, braking)

 Tech Stack
- Python
- FastF1
- Pandas
- Matplotlib
- Seaborn
- NumPy

  How to Run
1. Install dependencies:
   pip install fastf1 pandas matplotlib seaborn numpy
2. Open the notebook in Google Colab or Jupyter
3. Run all cells in order — session data loads automatically via FastF1
4. First run may take 1-2 minutes to download telemetry cache

  Data Source
FastF1 library pulls live timing and telemetry data directly from
the official Formula 1 data feed. No manual download required.
