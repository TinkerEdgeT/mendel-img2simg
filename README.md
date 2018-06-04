# What is this?

This is an extracted copy of the source of the libsparse library in the Debian
android-platform-system-core-7.0.0+r33 package, modified to only include the
libsparse tools and the system/core/include subtree of the Android source tree.

## Why did we make this fork?

We wanted to use img2simg/simg2img to manipulate images into sparse images and
back, but didn't want to depend on the entirety of the system/core subtree of
Android. Unfortunately, while the img2simg tools are available in Ubuntu Artful
and later, our internal systems currently only support Ubuntu Trusty, so we were
forced to build this tool from source.

As these tools are relatively minor in nature, it made sense to extract only the
sources that are used to build these tools and place them here to be integrated
with the rest of the build scripts.

Over time, this tool will be removed from the build entirely, and integrated
properly into the prereqs.
