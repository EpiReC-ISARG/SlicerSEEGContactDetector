# SEEG Contact Detector

**SEEG Contact Detector** is a 3D Slicer extension for automatic and highly accurate localization of intracerebral electrode contacts from post-implantation CT imaging.

**Stereoelectroencephalography (SEEG)** is an invasive diagnostic technique widely used in the presurgical evaluation of patients with drug-resistant focal epilepsy. Multiple depth electrodes are implanted into the brain to record electrical activity and identify the seizure onset zone. Accurate localization of individual electrode contacts is essential for the correct interpretation of SEEG recordings, planning of surgical interventions, and integration of electrophysiological data with anatomical imaging.

Traditionally, contact localization is performed manually by clinical experts through visual inspection of post-implantation imaging. This process is time-consuming, may require several hours per patient, and is susceptible to inter-operator variability. The task becomes particularly challenging when electrodes follow non-linear trajectories, converge with neighboring electrodes, or when some contacts are only partially visible because of CT artifacts.

SEEG Contact Detector automates this workflow by combining image segmentation, electrode trajectory estimation, and model-based contact fitting. The algorithm is designed to handle electrode bending, twisting, partial contact visibility, and imaging artifacts while respecting the physical dimensions of implanted electrodes. The extension provides both fully automatic detection and intuitive tools for quick visual review and manual correction when needed.

![Detection](docs/images/detection.gif)

📘 **See the documentation for details**
👉 https://epirec-isarg.github.io/SlicerSEEGContactDetector/

---

## Key Capabilities

- Automatic localization of SEEG contact centers from post-implantation CT
- Robust detection of thousands of contacts within minutes
- Model-based fitting that respects electrode geometry, contact length, and inter-contact spacing
- Accurate handling of curved electrode trajectories using 5th-degree polynomial modeling
- Integrated tools for quality control, visual review, and rapid manual correction
- Automatic brain mask generation from pre-implantation MRI when a CT brain mask is unavailable
- Detection of contacts with partial visibility caused by CT artifacts
- Tight integration with 3D Slicer workflows and visualization tools