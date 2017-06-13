# Current version

CUPS 2.2.1

# What is CUPS?

CUPS is an open source printing system that supports IPP along with other protocols. More information can be found at [cups.org](http://cups.org/)

# About this image

This image is based off [ticosax/cups-in-docker](https://github.com/ticosax/cups-in-docker) with a few specific tweaks:

* Debian testing is used as the base image. Most of the cups updates are put into testing fairly quickly so no need for unstable. This may change in future if versions start lagging behind.

# Running this image

```bash
docker run -e CUPS_USER_ADMIN=admin -e CUPS_USER_PASSWORD=secr3t -p 6631:631/tcp aadl/cups
```
