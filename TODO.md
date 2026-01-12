# Features
- [x] add registration
- [x] skull stripping
- [x] automatic installation of python packages
- [X] contact manual shifting
- [x] use cropped array around the balls for the correlation for faster computation
- [ ] ~~CT bone reconstruction~~
- [x] auto load input based on input file name
- [x] fiducial placement
- [x] use tip of the electrode instead of the linear approximation
- [x] add micro step while electrode shifting
- [x] new fiducial naming A-no, B-no
- [x] disabled buttons tooltip hint
- [ ] save curve in parameterNode
- [ ] electrode dimensions in Electrode class
- [x] electrodes output in T1 space
- [x] manual input -> disable metal check
- [x] skip registration button

# Visualization
- [x] debug checkbox to enable visualization
- [x] smaller cross marker after View in scene (test on Windows)
- [x] hide detections from previous run
- [x] set cross marker after Run

# Debugging
- [x] check centers of the spheres and of the gaussinan balls
- [x] test edge cases (bolt spheres around the edge of the image, gaussian balls around the edge of the image)
- [x] check algorithm on non standard spacing
- [x] fix memory leakage after deleting nodes from slicer
- [x] warning if there is no bolt around the input fiducial
- [x] fix error when extending the curve outside of the image / moving the electrode outside of the image
- [x] critical error when shifting contacts after renaming estimated contacts
- [ ] ~~cannot make window smaller due to the minimum size of the widgets => make Inputs buttons in vertical layout?~~
- [x] change estimation of the electrode axis orientation
- [x] start without extending the curve
- [x] ras tip fiducial naming C1-no to C1
- [x] save CT brain mask path is missing when T1 and CT are loaded outside of the module
- [x] CT path bug
- [x] electrode with zero length (A-0)

# Finalization
- [x] add parameters into the parameter node and check scene saving
- [x] remove step-by-step, add event on run all click
- [x] create tooltip help
- [ ] add module description, help and acknowledgement
- [x] icon
- [x] mrml scene (ocean, etc)
- [x] Sample data (defaced)
- [x] Tests
- [x] Documentation
- [x] GitHub description
- [ ] Check CMakeLists
- [x] Unify extension and module names
- [ ] EN short video
- [x] EN documentation

# Testing
- [x] prepare dataset
- [x] apply dummy affine transform to the T1
- [x] estimate bolt tip as extrapolation of the first and last contact and apply additional random translation away from the axis
- [x] evaluation script
- [x] batch loading (as a test function?)

# Known issues
- [x] while fitting the electrode with less than 5 contacts, out of range warning is raised