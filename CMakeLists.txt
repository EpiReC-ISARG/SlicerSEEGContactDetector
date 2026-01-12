cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(SlicerSEEGContactDetector)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://epirec-isarg.github.io/SlicerSEEGContactDetector/")
set(EXTENSION_CONTRIBUTORS "Jakub Smid (CTU in Prague, Charles University), Radek Janca (CTU in Prague)")
set(EXTENSION_DESCRIPTION "SEEG Contact Detector is a 3D Slicer extension for automatic localization of SEEG electrode contact centers from post-implantation CT data. The module uses a model-based approach that respects electrode geometry and accounts for bending, twisting, and partial contact visibility. It supports optional MRI-based brain masking, manual correction tools, and interactive visualization for efficient clinical review.")
set(EXTENSION_ICONURL "https://raw.githubusercontent.com/EpiReC-ISARG/SlicerSEEGContactDetector/refs/heads/master/ContactDetector.png")
set(EXTENSION_SCREENSHOTURLS "https://raw.githubusercontent.com/EpiReC-ISARG/SlicerSEEGContactDetector/refs/heads/master/Screenshot01.png https://raw.githubusercontent.com/EpiReC-ISARG/SlicerSEEGContactDetector/refs/heads/master/Screenshot02.png")
set(EXTENSION_DEPENDS "HDBrainExtractionTool") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(SEEGContactDetector)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
