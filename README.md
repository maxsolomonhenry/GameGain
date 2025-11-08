# Game Gain
Experiment wrapping the Wwise audio engine in JUCE so I can code a plugin on my MacOS.

## Learnings
- In `CMakeLists.txt` you need to add a second argument to `add_subdirectory()` when you are referencing something outside of the source tree (e.g., "../../something") because cmake typically mirrors the directory structure in the build directory. So when you reference outside of the tree, it's not sure where to put it in the build dir.
- Best practice to compile separate concerns individually and then link against those targets (e.g., Wwise vs. JUCE).