# AI-Guided Hardware-Aware Quantum Transpilation

A prototype hardware-aware quantum transpilation framework focused on reducing SWAP count, circuit depth, and improving execution reliability on superconducting quantum hardware.

## Overview

This project explores ML-guided qubit layout optimization and topology-aware transpilation for IBM heavy-hex architectures.

The system was benchmarked against:
- Qiskit
- IBM AI Routing
- SABRE

using identical circuits, hardware topology, calibration data, and random seeds.

## Benchmark Setup

- IBM heavy-hex hardware topology
- Live calibration-based backend data
- 20–25 logical qubits
- Topologies tested:
  - Line
  - Cycle
  - Star
  - Random
  - Complete

Metrics evaluated:
- SWAP count
- Circuit depth
- Estimated Success Probability (ESP)

## Results

### Total SWAP Count ↓

| System | SWAPs |
|---|---|
| My AI | 2037 |
| Qiskit | 2285 |
| IBM AI | 2269 |
| SABRE | 2276 |

### Total Circuit Depth ↓

| System | Depth |
|---|---|
| My AI | 3813 |
| Qiskit | 4112 |
| IBM AI | 3600 |
| SABRE | 4184 |

### Average Estimated Success Probability ↑

| System | ESP |
|---|---|
| My AI | 0.1584 |
| Qiskit | 0.0617 |
| IBM AI | 0.0641 |
| SABRE | 0.0843 |

## Key Ideas

- Hardware-aware layout optimization
- ML-guided transpilation
- Noise-aware routing evaluation
- Heavy-hex topology optimization
- Calibration-aware execution scoring

## Technologies

- Python
- Qiskit
- NetworkX
- IBM Quantum backend data

## Benchmark Report

Full benchmark methodology and results:

`benchmark_results.pdf`

## Research Interests

Quantum Compilation • Machine Learning for Quantum Systems • Hardware-Aware Optimization • Quantum Architecture
