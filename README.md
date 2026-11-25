# DFT

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Rusher3265/DFT/blob/main/Tantalum_DFT_Colab.ipynb)

A self-contained notebook for bulk alpha-tantalum DFT, phonons, electron–phonon coupling and superconductivity analysis with Quantum ESPRESSO 7.5 and EPW 6.0.

## Run in Google Colab

1. Click **Open in Colab** above.
2. Select a **Python 3 CPU runtime**.
3. Save a copy of the notebook to Google Drive.
4. Run notebook sections **1–5 in order** for installation, input downloads, checkpoints and the first DFT calculation.
5. Enable the later `RUN_...` switches for convergence, electronic properties, phonons and EPW. Repeat the phonon chunk cell until complete.
6. Use the final cells to download the analysis report. After a runtime reset, rerun sections **1–3** with the same project paths to restore the latest Drive checkpoint.

All Python source is embedded in the notebook; no separate source download or API key is needed for the default workflow.

## Scientific scope

The model is bulk, nonmagnetic bcc alpha-Ta at ambient pressure. Pilot settings require numerical convergence before interpreting a predicted transition temperature. Normal-state DFT bands do not contain a superconducting gap. Thin films, beta-Ta, disorder, oxides and device losses need additional models.

The notebook includes scalar and SOC input generation, bands/DOS/PDOS, energy-volume fitting, DFPT phonons, independent EPW interpolation checks, Eliashberg spectra, Allen–Dynes sensitivity analysis, optional isotropic imaginary-axis gap calculations, reports and Drive checkpoints.

The recreated implementation passed 38 Python tests and real scalar-relativistic QE/EPW pilot calculations. A signed-in Colab session and the full SOC electron–phonon chain were not exercised during verification. Detailed provenance and validation notes are embedded with the source.
