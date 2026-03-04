# ERIP

A data collection and analysis project built around **Risk of Rain 2** gameplay sessions.

## Project Structure

- **RoR2/** — C# BepInEx mod (`ScienceKit`) that hooks into the game and records in-game stats in real time.
- **Python/** — scripts for cleaning, joining, and aggregating the raw data collected by the mod.
- **DATASET.csv** — the final dataset ready for analysis.

## How It Works

The `ScienceKit` mod runs alongside the game and captures telemetry data during each session.
That raw data is then processed through the Python pipeline — converted, merged, and aggregated — producing the structured `DATASET.csv`.
