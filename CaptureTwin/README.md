# Capture Twin

![image](image/Capture_twin.png)

A *captured twin* is a digital replica of a physical object,
created using data from sensors or cameras. In Reality Composer,
this process, known as  *3D Capture*, involves taking multiple
images of an object from different angles and using
*photogrammetry* to combine them into a 3D model. These models
can then be imported into Reality Composer projects, allowing
users to interact with them in AR environments.

* _Use Case_: Virtual Object Replica
* _Technology Platform_: [Reality Composer](../README.md)
* _Device Type_: handheld
* _Vision System_: world camera

## 3D Object Capture

<img src="image/3D_capture.jpg" width="450"/>

Apple's Reality Composer uses the "Object Capture" feature to create realistic
3D models from photographs. To achieve optimal results, position the object in a well-lit
environment with even lighting to minimize shadows. Adjust the capture frame to fully enclose
the object, then move your device around it slowly to capture images from multiple angles,
ensuring complete coverage for photogrammetry.

<img src="image/Interface.png" width="220"/> <img src="image/Interface2.jpg" width="189"/> <img src="image/Interface3.jpg" width="190"/>

The app processes these images to generate a detailed 3D
model, which can be viewed, manipulated, or used in AR.
Models can be saved as USDZ files for cross-platform
compatibility or reprocessed on a Mac for enhanced quality.

## Captured Twin Ahead Staging

<img src="image/Aromat_twin.png" width="240"/> <img src="image/Bottle.png" width="251"/>

### AR Patterns

__Behavior Pattern__

* [Instant Reaction](https://github.com/ARpatterns/catalog/blob/main/behavioral-patterns/instant-reaction.md):
  Immediate execution of the staging ahead action upon import of the captured twin.
  * _Event_: On floor detection.

__Augmentation Pattern__

* [Ahead Staging](https://github.com/ARpatterns/catalog/blob/main/augmentation-patterns/ahead-staging.md): Presenting the captured 3D twin object in front of the user.
  * _Placed_: Initial ahead of the user on the floor next to the original.
  * _Aligned_: Initial towards the user in view direction.
  * _Pivot_: Reality Composer objects in the local coordinate system are centered on the ground floor.

### ECA Diagram

| on:command | &rarr; | do:import |
| ---------- | ------ | --------- |

> 'Bottle' ➕

| on:command | &rarr; | do:add ahead |
| ---------- | ------ | ------------ |

> 'Bottle' ➕

## References
> [!TIP]
> Try out the examples: Download and try the files in [ProjectExamples](CaptureTwin/ProjectExamples) for your AR experience with your own iOS device.

- Apple Reality Composer [App](https://apps.apple.com/us/app/reality-composer/id1462358802)
- ECA [Diagram](https://github.com/ARpatterns/diagram)