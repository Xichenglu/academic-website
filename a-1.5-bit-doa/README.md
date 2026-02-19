# A 1.5-Bit Quantization Demo for DOA Estimation

This repository contains a MATLAB demo implementation for low-bit quantization based DOA estimation with MUSIC.

It is organized as a clean and reproducible baseline corresponding to:

> X. Lu, W. Liu, and A. Alomainy, "A 1.5-Bit Quantization Scheme and Its Application to Direction Estimation," *IEEE Transactions on Signal Processing*, 2025.

## Project structure

- `run_music_15bit_demo.m` — main demo script.
- `functions/` — reusable helper functions:
  - signal generation and steering matrix,
  - b-bit quantizer,
  - Van Vleck style correlation recovery,
  - MUSIC spectrum and peak extraction.
- `CITATION.cff` — citation metadata.
- `LICENSE` / `COPYRIGHT` — license and copyright notice.

## Requirements

- MATLAB R2021a+ (recommended)
- Signal Processing Toolbox (for `findpeaks`)

## Quick start

1. Open MATLAB and navigate to this folder.
2. Run:

```matlab
run_music_15bit_demo
```

3. Adjust parameters at the top of the script (e.g., `SNR_dB`, `b`, `lambda`, `theta`) and rerun.

## Notes

- Set `b = 2` for the 1.5-bit style quantization experiment.
- A fixed random seed is included for reproducibility.
- This code is provided for research and educational use.

## Citation

If this code helps your research, please cite the paper above. You can also use metadata in `CITATION.cff`.

## Contact

For questions or collaboration, please contact Xicheng Lu via your academic contact channel.
