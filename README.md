# SEEG Contact Detector

**SEEG Contact Detector** is a 3D Slicer extension for automatic and accurate localization of SEEG electrode contact centers from post-implantation CT data. The extension is designed to handle electrode bending, twisting, and partial contact visibility while respecting the physical electrode model.

![Detection](docs/images/detection.gif)

📘 **See the documentation for details**
👉 https://epirec-isarg.github.io/SlicerSEEGContactDetector/

---

## Key Capabilities

- Automatic detection of SEEG contact centers from post-implantation CT
- Model-based approach respecting electrode length and inter-contact spacing
- Robust handling of electrode bending and twisting using 5th-degree polynomial fitting
- Support for manual corrections (manual electrode tip, contact shifting, microsteps)
- Tight integration with 3D Slicer workflows and visualization tools