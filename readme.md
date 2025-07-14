# Low-Latency Implementation of Bitsliced SPN-Cipher on IoT Processors

This repository contains the implementation and evaluation framework for optimizing bitsliced SPN-cipher implementations on 32-bit processors like ARM Cortex-M4. The work focuses on both theoretical optimization techniques and practical performance evaluation.

## Contents

The project consists of three main components:

- `non-linear-layer`: Implementation of a novel S-box optimization technique using the Bit-slice Gate Complexity (BGC) model that improves the efficiency of the non-linear substitution layer.
- `linear-layer`: Implementation of the Optimization of Permutation Operations (OPO) algorithm for optimizing the linear permutation layer. The key implementation is in [optimize_permutation.ipynb](linear-layer/optimize_permutation.ipynb).
- `LCB`: A comprehensive benchmarking framework for evaluating lightweight block cipher implementations on microcontrollers. Contains the experimental data and performance measurements discussed in the paper.

## Getting Started

- See `non-linear-layer/readme.md` for S-box optimization
- See `linear-layer/readme.md` for permutation optimization
- See `LCB/README.md` for performance evaluation framework

## Tested Platforms

The optimizations target 32-bit microcontroller platforms:

- ARM Cortex-M4 based boards (STM32L475)
- ESP32-S3 based boards
