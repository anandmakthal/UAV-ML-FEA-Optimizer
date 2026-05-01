
### ML-Driven UAV Frame Structural Optimizer
**Anand Makthal | MS Aerospace & Mechanical Engineering | Saint Louis University | 2026**

---

## Project Summary
A closed-loop system combining real UAV flight telemetry, 
SOLIDWORKS FEA structural analysis, and a neural network 
to automatically optimize UAV frame geometry.

## Real Results
| Design | Stress | FOS | Status |
|--------|--------|-----|--------|
| Baseline (3mm, 180mm) | 572.2 MPa | 0.48 | FAIL |
| Optimized (6mm, 160mm, 35mm root) | 53.81 MPa | 5.11 |  PASS |

**90% stress reduction achieved through ML-guided optimization!**

## Tools Used
- SOLIDWORKS 2024 — CAD + FEA Simulation
- Python — Data extraction + Neural Network
- PX4 Flight Logs — Real UAV telemetry (50.91N loads)
- PyTorch — Neural network (R²=0.9788, 97.88% accuracy)

## Neural Network Performance
- Architecture: 4→64→32→1 feedforward network
- Training: 1000 epochs, Adam optimizer
- R² Score: 0.9788 (97.88% accuracy)
- Dataset: 17 FEA runs (2 real SOLIDWORKS + 15 physics-based)

## Project Workflow
1. Extract structural loads from real PX4 UAV telemetry
2. Build UAV frame in SOLIDWORKS (CenterBody + 4 Arms)
3. Run FEA with real flight loads (50.91N per motor)
4. Train neural network on FEA dataset
5. ML optimizer scans 1000+ designs in seconds
6. Validate optimal design in SOLIDWORKS FEA

## Author
**Anand Makthal**
MS Aerospace & Mechanical Engineering
Saint Louis University | May 2026

