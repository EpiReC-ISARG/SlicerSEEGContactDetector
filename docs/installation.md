# Installation

## Option 1: Installation via Extension Manager

The recommended way to install the SEEG Contact Detector extension is through the 3D Slicer Extension Manager. This is the preferred method for end users.

1. In 3D Slicer, navigate to **View → Extension Manager**.
2. Open the **Install Extensions** tab and search for SEEG Contact Detector.
3. Click **Install**, then restart 3D Slicer when prompted.
4. The SEEG Contact Detector module will then appear in the list of available modules.

For quicker access, the module can be added to the toolbar. Navigate to **Edit → Application Settings → Modules**, locate *SEEG Contact Detector* in the module list, and drag and drop it into the **Favorite Modules** section. The module icon will then appear in the toolbar.

## Option 2: Using Source Code
This method allows you to install the extension directly **without using the Extension Manager** and is the **recommended approach for development.**

### Dependencies
SEEG Contact Detector depends on one external module that must be installed **manually via the 3D Slicer Extension Manager** before loading this extension. If this dependency is missing, SEEG Contact Detector will not load correctly.

Please ensure that the following extension is installed:

* [HDBrainExtraction](https://github.com/lassoan/SlicerHDBrainExtraction)

### Load the Extension
1. Download the source code from GitHub: [https://github.com/EpiReC-ISARG/SlicerSEEGContactDetector](https://github.com/EpiReC-ISARG/SlicerSEEGContactDetector).
It is recommended to use a [stable release](https://github.com/EpiReC-ISARG/SlicerSEEGContactDetector/releases) or the latest commit on the main branch that represents the current stable version.
2. Unzip the downloaded archive.
3. Launch 3D Slicer and drag-and-drop the folder containing the extension source code into the 3D Slicer application window.
4. When prompted, select `Add Python scripted modules to the application`.
5. The SEEG Contact Detector module will be added to the list of available modules without requiring a restart of 3D Slicer.
6. When you start detection first time, you will be prompted to install the externa

If needed, you can later modify the extension path in: Edit → Application Settings → Modules → Additional module paths.