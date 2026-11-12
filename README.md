# jcicaaa3

[日本語](README_JA.md) · [한국어](README_KO.md)

Computer engineering student at Hankuk University of Foreign Studies, double majoring in Northeast Asian Diplomacy and Commerce. I work on security and machine learning together: I analyze Windows ransomware, and I am starting on ML-based malware detection.

[Site](https://jcicaaa3-cloud.github.io/en/) · [Posts](https://jcicaaa3-cloud.github.io/en/research/) · [Projects](https://jcicaaa3-cloud.github.io/en/projects/) · [jcicaaa3@gmail.com](mailto:jcicaaa3@gmail.com)

## Malware analysis

### Calipso ransomware (2026)

Static analysis in Ghidra. The write-up covers the encryption design (XChaCha20 over the first 5MB of each file, session key wrapped with RSA-4096 OAEP), file discovery by enumerating the MFT directly (`FSCTL_ENUM_USN_DATA`), recovery inhibition such as shadow copy and event log deletion, and IOCs, a YARA rule, and MITRE ATT&CK mapping.

[Analysis v2.0](https://jcicaaa3-cloud.github.io/en/research/calipso-v2/) · [Screenshots](https://jcicaaa3-cloud.github.io/en/evidence/)

Malware samples are never uploaded to public repositories.

## Projects

### [LiteRaceSegNet](https://github.com/jcicaaa3-cloud/LiteRaceSegNet-FINAL-)

A 0.125M-parameter CNN for road-damage segmentation with a boundary head. Validation mIoU 0.807 on 10 images, 3.1 ms/image on CUDA, and a 7-variant ablation. Edge quality is still weak (test boundary F1 0.058), and the README says so.

### [HPLS-Eval](https://github.com/jcicaaa3-cloud/HPLS-Eval-v0.2.7)

An evaluation tool for small-mask segmentation across runtimes (CPU, GPU, NPU, TPU) and precisions (FP32, FP16, INT8). It checks which execution provider actually ran and whether an INT8 model is really quantized.

### [Financial Risk Scoring](https://github.com/jcicaaa3-cloud/financial-risk-scoring-service-FINAL)

An ML backend that scores three next-quarter risk signals from quarterly company data: input validation, time-ordered evaluation, FastAPI, and monitoring reports. Synthetic data only.

### [MachiLens](https://github.com/jcicaaa3-cloud/machilens-shibuya-ai-predictor)

A BiLSTM model that compares urban strategy scenarios for Shibuya on synthetic data, rebuilt from a class project. The random forest baseline beats it, and the README shows both.

### Robot action success/failure evaluation

A research project from spring 2026 on how to judge whether a robot completed a task. I analyzed 874 cases from 80 runs and looked at how the verdict changes with the judging criterion. [Summary](https://jcicaaa3-cloud.github.io/en/projects/robot-evaluation/)

## Tools

- Malware analysis: Ghidra, YARA, MITRE ATT&CK, Python, PowerShell
- ML and computer vision: PyTorch, scikit-learn, OpenCV, NumPy, Pandas
- Development: Git, Linux, FastAPI, Docker, GitHub Actions

## Contact

[jcicaaa3@gmail.com](mailto:jcicaaa3@gmail.com)
