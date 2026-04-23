# ICASSP 2026:

**Title:** Improving Automatic Speech Recognition by Mitigating Distortions Introduced by Speech Enhancement Under Drone Noise

**Authors:** Ryusei Miura, Takahiro Osaki, Benjamin Yen, Takeshi Ashizawa, Kazuhiro Nakadai

[Back to Home](../index.md)

---

## Word Error Rate (WER) Results (Additional)
Although the character error rate (CER) is included in the paper, the comparison results for the word error rate (WER) in each drone noise environment are presented here.

**Table 1: Comparison of ASR performance in word error rate (WER) [%] under various drone noise conditions at 0 / -5 / -10 dB SNR.** Results are shown for three drone noises (Bebop, Mambo, MK-Quadro) and their average. Bold indicates the best result for each noise condition, with the final proposed system also highlighted.

| System | Bebop <br> (0 / -5 / -10 dB) | Mambo <br> (0 / -5 / -10 dB) | MK-Quadro <br> (0 / -5 / -10 dB) | Average <br> (0 / -5 / -10 dB) |
| :--- | :---: | :---: | :---: | :---: |
| ASR Only | 62.4 / 87.4 / 98.1 | 50.1 / 75.2 / 92.0 | 49.6 / 64.0 / 95.7 | 54.0 / 75.5 / 95.3 |
| Conv-TasNet | 51.3 / 84.1 / 102.7 | 47.7 / 76.0 / 92.7 | 41.4 / 78.6 / **94.4** | 46.8 / 79.6 / 96.6 |
| MossFormer | 43.0 / 63.8 / **87.4** | 40.6 / 61.7 / **84.1** | 45.4 / 76.4 / 94.8 | 43.0 / 67.3 / **88.8** |
| DM (SGMSE+) | 48.4 / 77.1 / 96.1 | 30.9 / 52.5 / 81.8 | 40.6 / 95.4 / 120.5 | 40.0 / 75.0 / 99.5 |
| Conv-TasNet + BN | 39.2 / 72.2 / 131.1 | 37.8 / 66.4 / 126.0 | 28.9 / 62.9 / 107.1 | 35.3 / 67.2 / 121.4 |
| MossFormer + BN | 41.2 / **61.9** / 90.9 | 33.6 / 50.0 / 77.9 | 35.7 / 68.7 / 99.9 | 36.8 / 60.2 / 89.6 |
| DM + BN | 41.1 / 70.9 / 169.4 | 26.9 / 48.9 / 147.1 | 28.5 / 63.8 / 101.3 | 32.2 / 61.2 / 139.3 |
| DM + FF | 39.8 / 71.9 / 96.1 | 24.8 / 47.2 / 79.8 | 32.7 / 84.3 / 116.9 | 32.4 / 67.8 / 97.6 |
| DM + (S5, S6, S6) | 39.8 / 70.2 / 93.7 | 26.1 / 50.5 / 82.2 | 33.1 / 75.4 / 100.1 | 33.0 / 65.4 / 92.0 |
| DM + AFM | 39.8 / 72.2 / 95.4 | 25.1 / 47.4 / 78.9 | 32.4 / 83.0 / 116.2 | 32.4 / 67.5 / 96.8 |
| DM + FF + BN | **37.4** / 67.8 / 169.9 | **24.6** / **45.9** / 102.4 | **26.3** / **62.2** / 142.0 | **29.4** / **58.6** / 138.1 |
| DM + (S5, S6, S6) + BN | 39.1 / 73.0 / 176.1 | 27.6 / 55.3 / 155.7 | 29.4 / 68.4 / 167.8 | 32.0 / 65.6 / 166.5 |
| **DM + AFM + BN** | **37.4** / 67.2 / 151.4 | **24.6** / 46.9 / 104.7 | **26.3** / 63.1 / 135.4 | **29.4** / 59.1 / 130.5 |