# MiSTer Docker Development

This repository is a bootstrap for developers to get several containers up and running for MiSTer development.

# Main_MiSTer Docker Development Setup and Compile

From the Main_MiSTer folder, Issue this command to pull down a working linaro toolchain docker image, and cross compile the code:
```
docker run -ti -v $(pwd):/source wsbu/toolchain-linaro bash -c "cd /source; make BASE=/opt/linaro/bin/arm-linux-gnueabihf"
```
Thanks to inagy for figuring this out!
