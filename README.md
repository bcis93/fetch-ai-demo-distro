# fetch-ai-demo-distro
Demo distrubution for the [meta-fetch-ai](https://github.com/bcis93/meta-fetch-ai) layer.

The following layers are included as submodules of this project:
- poky
- meta-openembedded
- meta-virtualization
- meta-fetch-ai
- meta-raspberrypi

## Dependencies and Environment

Refer to [Yocto Project Quick Build](https://docs.yoctoproject.org/brief-yoctoprojectqs/index.html) for a list of dependencies and system
compatibility information.

## Getting Started

Run the following commands to clone the repository and start a build!
```
git clone git@github.com:bcis93/fetch-ai-demo-distro.git
cd fetch-ai-demo-distro
git submodule update --init
source layers/poky/oe-init-build-env
bitbake core-image-base
```

## Current Status

Currently, the build succeeds, and running `aea` on the target device runs without errors.

The following list describes the tasks to be completed next:
- Add an example of how to deploy an AEA with the build (once this task is finished in meta-fetch-ai).
- Create a 'dev' image with git, ssh, and other similar features installed.
- Add another distro with mender support. This will enable easy OTA updates.


## Issues and Contributing

If you encounter a build or run-time issue or would like to contribute, please create an issue or submit a pull request. Contributions are appreciated!
