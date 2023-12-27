
# EPFL Rocket Team - Project Tiroir

This organization contains all the repositories for our team in the 4th Space Race of the EPFL Rocket Team.

# Avionics

We developped some telemetry tools and some radio transmission software to communicate between our avionics board and our ground station.

To do this, we implemented :
 - [raspberry-pi-sdk](https://github.com/ert-tiroir/raspberry-pi-sdk), a library to handle GPIO, I2C and a few other tools on a Raspberry PI, also providing a virtual version of the software to allow us to simulate trajectories.
 - [wsserver](https://github.com/ert-tiroir/wsserver), a tiny web socket server in C++ for our ground station to communicate with our browser interface.
 - [tiroir-software](https://github.com/ert-tiroir/tiroir-software), our Avionics software that uses our custom Raspberry PI SDK.

# Video Software

One of the main goals of the Avionics Team was to have an on board camera with live retransmission to our ground station. To do that, we created two main repositories :
 - [wsserver-video](https://github.com/ert-tiroir/wsserver-video), a video broadcaster and video player based on our tiny web socket server.
 - [wsserver-video-ffmpeg](https://github.com/ert-tiroir/wsserver-video-ffmpeg), an extension of our video broadcaster to apply a FFMPEG middleware on, either to transcode a video stream or to create one from a growing set of images
