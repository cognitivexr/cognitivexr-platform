CognitiveXR Platform
====================

This repository contains links to the core CognitiveXR platform components.
There are two major components:

* [CPOP Server](https://github.com/cognitivexr/cpop)

  The Cyber-Physical Object Positioning (CPOP) system is responsible for perceiving the environment, translating the coordinates of objects in the environment into 3D coordinates, and sending them to nearby devices so can be displayed.
  This allows, for example, pedestrians to see cars that are outside their own field of view, but in the field of view of a nearby camera.

* [CogStream](https://github.com/cognitivexr/cogstream)

  CogStream is the video offloading platform that allows low-compute AR devices to perform complex AI-based analytics tasks.
  AR devices can annotate their own field of view by offloading their camera stream to CogStream to detect things like objects, faces and their emotions, or hand signs.
  The CogStream mediator negotiates a streaming format between the Analytics Engine and the client requesting a particular analytics capability.
  The mediator then creates new instances of analytics engines, and instructs clients to connect to them.
  Clients then offload their video to the engine, which processes the stream frame-by-frame, and returns the annotations the engine can detect (e.g., faces, or objects).

The following figure shows an example interaction.
Highlighted components are part of the platform.

<p align="center">
  <img src="https://raw.githubusercontent.com/cognitivexr/cognitivexr-platform/master/images/cognitivexr-platform.png" alt="CognitiveXR Platform Components">
</p>
