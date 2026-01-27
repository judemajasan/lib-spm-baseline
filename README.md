# Project 1 — Baseline Single Particle Model (SPM) in PyBaMM

## Objective
I run a physics-based Li-ion SPM using PyBaMM and reproduce a 1C discharge voltage curve, cutoff voltage: 2.7 V using Chen2020 parameters
## Result
![SPM 1C discharge](figures/spm_1C_discharge.png)

## Notes
SPM resolves lithium diffusion inside representative particles and reaction kinetics,
but neglects electrolyte concentration gradients and electrode-thickness gradients.
This would naturally make it less accurate at high C-rates vs SPMe/DFN.

## Project 2 — SPM vs SPMe across C-rate

**Question:** When does electrolyte physics matter?

I compared SPM (solid diffusion + kinetics) vs SPMe (adds electrolyte transport) for discharge at 0.5C, 1C, 2C, 3C using Chen2020 parameters.
