--- 
title: vTouch
---

# vTouch

VTouch is a multitouch browser frontend for Ableton Live. Inside your
webbrowser you can control clip triggering, volume, send and return
levels, mute, solo, record states. This works also on the network, so
you can connect your mobile phone, iPads or android tablets easily by
just browsing to you local webserver.

<p><iframe width="425" height="349" src="http://www.youtube.com/embed/qFmiIcgRIao" frameborder="0" allowfullscreen></iframe></p>


### About the Hack

Ableton Live is an digital audio workstation, which is well suited for
live performances. Lots of parameters can be manipulated, midi or
audio loops can be triggered. Unfortunately it is cumbersome to use
this software with a touch device. A user interface specifically
designed to be used on multitouch devices, which is also portable
across platforms, offers many benefits and possibilities. Imagine a
whole band jamming on iPads with ohne live setup over a wireless
network.


### Technology used

The frontend is rendered on HTML5 Canvas and communicates with a
nodejs server via websockets. On the backend the webserver talks to a
running ableton live instance and sends updates to all connected
clients.

The canvas frontend is supported on all modern browsers including
apple mobile safari and android browsers. We created a small widget
library named canvas.ui to take care of multitouch events, rendering
and layout management.
