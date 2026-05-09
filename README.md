# Quick Start
* The following commands demonstrate how to set up a new Yocto workspace,
* initialize the manifest repository, synchronize all layers, configure
* the build environment, and build/run a reference image.
```
$ mkdir <workspace>                                                 # Create a new workspace directory
$ cd <workspace>                                                    # Enter the workspace
$ repo init -u https://github.com/practice-yocto/manifest-core.git  # Initialize repo with the manifest
$ repo sync                                                         # Fetch all layers defined in the manifest
$ source envsetup.sh                                                # Set up the Yocto build environment
$ bitbake core-image                                                # Build the core-image target
$ runqemu core-image nographic                                      # Run the image in QEMU (no graphics)
```