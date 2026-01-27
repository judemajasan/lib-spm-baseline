# Project 1 — Baseline Single Particle Model (SPM) in PyBaMM

## Objective
Run a physics-based Li-ion SPM using PyBaMM and reproduce a 1C discharge voltage curve.

## Model & Parameters
- Model: pybamm.lithium_ion.SPM()
- Parameter set: Chen2020

## Experiment
- Constant-current discharge at 1C
- Cutoff voltage: 2.7 V

## Result
![SPM 1C discharge](figures/spm_1C_discharge.png)

## Notes
SPM resolves lithium diffusion inside representative particles and reaction kinetics,
but neglects electrolyte concentration gradients and electrode-thickness gradients.
This would naturally make it less accurate at high C-rates vs SPMe/DFN.
