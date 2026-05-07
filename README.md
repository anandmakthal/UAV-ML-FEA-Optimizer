# ML-Driven Adaptive UAV Frame Optimizer
### Integrating Real Flight Telemetry · SOLIDWORKS FEA · Neural Networks · Fluid Mechanics

**Anand Makthal | MS Aerospace & Mechanical Engineering | Saint Louis University | May 2026**

## Project Summary

A closed-loop machine learning system that combines real UAV flight telemetry, 
SOLIDWORKS FEA, a Neural Network stress predictor, and a Random Forest 
aerodynamic drag model to automatically optimize UAV quadcopter frame geometry.


## Real SOLIDWORKS FEA Results

| Design | Thickness | Length | Root Width | Fillet | Max Stress | FOS | Status |
|--------|-----------|--------|------------|--------|------------|-----|--------|
| Design 1 — Baseline | 3mm | 180mm | 20mm | 0mm | **572.2 MPa** | 0.48 |  FAIL |
| Design 2 — Improved | 5mm | 180mm | 40mm | R20mm | **75.12 MPa** | 3.66 |  PASS |
| Design 3 — Optimized | 6mm | 160mm | 50mm | R25mm | **54.46 MPa** | 5.05 |  PASS |
| Design 4 — ML Validated  | 8.5mm | 200mm | 25mm | R10mm | **50.46 MPa** | 5.45 |  BEST |

> **91.2% stress reduction from baseline to ML-validated design!**


## Complete Closed-Loop Pipeline
