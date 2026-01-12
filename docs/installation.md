# Installation

## Option 1: Using Source Code
This method allows you to install the extension directly **without using the Extension Manager** and is the **recommended approach for development.**

### Dependencies
SEEG Contact Detector depends on one external module that must be installed **manually via the 3D Slicer Extension Manager** before loading this extension. If this dependency is missing, SEEG Contact Detector will not load correctly.

Please ensure that the following extension is installed:

* [HDBrainExtraction](https://github.com/lassoan/SlicerHDBrainExtraction)

### Load the Extension
1. Download the source code from GitHub: [https://github.com/EpiReC-ISARG/SlicerSEEGContactDetector](https://github.com/EpiReC-ISARG/SlicerSEEGContactDetector).
It is recommended to use a stable release or the latest commit on the master branch that represents the current stable version.
2. Unzip the downloaded archive.
3. Launch 3D Slicer and drag-and-drop the folder containing the extension source code into the 3D Slicer application window.
4. When prompted, select `Add Python scripted modules to the application`.
5. The SEEG Contact Detector module will be added to the list of available modules without requiring a restart of 3D Slicer.
6. When you start detection first time, you will be prompted to install the externa

If needed, you can later modify the extension path in: Edit → Application Settings → Modules → Additional module paths.

## Option 2: Installation via Extension Manager (planned)