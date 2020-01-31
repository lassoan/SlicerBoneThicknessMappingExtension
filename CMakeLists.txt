cmake_minimum_required(VERSION 3.5)

project(Bone Thickness Mapping)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "http://slicer.org/slicerWiki/index.php/Documentation/Nightly/Extensions/BoneThicknessMapping")
set(EXTENSION_CATEGORY "Shape Analysis")
set(EXTENSION_CONTRIBUTORS "Evan Simpson (HML & SKA Lab, Western University)")
set(EXTENSION_DESCRIPTION "This is an example of a simple extension")
# set(EXTENSION_ICONURL "http://www.example.com/Slicer/Extensions/ThicknessMapping.png")
# set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/BoneThicknessMapping/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(BoneThicknessMapping)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})