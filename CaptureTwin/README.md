# Captured Twin

![image](image/Capture_twin.png)

A captured twin is a digital replica of a physical object, created using data from sensors or cameras. In Reality Composer, this process, known as  3D Capture, involves taking multiple images of an object from different angles and using photogrammetry to combine them into a 3D model. These models can then be imported into Reality Composer projects, allowing users to interact with them in AR environments.

* _Use Case_: Virtual Object Replica
* _Technology Platform_: [Reality Composer](../README.md)
* _Device Type_: Handheld
* _Vision System_: World camera

## 3D Object Capture

<img src="image/3D_capture.jpg" width="450"/>

Apple's Reality Composer uses the "Object Capture" feature to create realistic
3D models from photographs. To achieve optimal results, position the object in a well-lit
environment with even lighting to minimize shadows. Adjust the capture frame to fully enclose
the object [PictureOfMouse1](image/Interface.png), then move your device around it slowly to capture images from multiple angles [PictureOfMouse2](image/Interface2.jpg),
ensuring complete coverage for photogrammetry [PictureOfMouse3](image/Interface3.jpg).

<img src="image/Interface.png" width="219.5"/> <img src="image/Interface2.jpg" width="189"/> <img src="image/Interface3.jpg" width="191"/>

The app processes these images to generate a detailed 3D
model, which can be viewed, or used in AR.
Models can be saved as USDZ files for cross-platform
compatibility or reprocessed on a Mac for enhanced quality.

## Captured Twin Instant Ahead Staging

<img src="image/Aromat_twin.png" width="240"/> <img src="image/Bottle.png" width="251"/>

### AR Patterns

__Behavior Pattern__

* [Instant Reaction](https://github.com/ARpatterns/catalog/blob/main/behavioral-patterns/instant-reaction.md): After Object Capture and import of the captured twin. Immediate execution of the staging ahead action upon detection of the horizontal plane as anchorage point.
  * _Event_: Horizontal plane detection.

__Augmentation Pattern__

* [Ahead Staging](https://github.com/ARpatterns/catalog/blob/main/augmentation-patterns/ahead-staging.md): Presenting the captured 3D twin object as virtual dublicate beside the real one.
  * _Placed_: Initial ahead of the user immediately upon achor point detection.
  * _Pivot_: Reality Composer objects in the local coordinate system are centered on the anchorage point.

### ECA Diagram

| on:command | &rarr; | do:import to project |
| ---------- | ------ | -------------------- |

> 'Aromat' ⬇️

| on:click | &rarr; | do:add ahead |
| -------- | ------ | ------------ |

> 'Aromat' ➕

| on:command | &rarr; | do:import to project |
| ---------- | ------ | -------------------- |

> 'Bottle' ⬇️

| on:command | &rarr; | do:add ahead |
| ---------- | ------ | ------------ |

> 'Bottle' ➕

## References

> [!TIP]
> Try out the examples: Download and try the files in [ProjectExamples](https://github.com/ARpatterns/AppleRealityComposer/tree/main/CaptureTwin/ProjectExamples) for your AR experience with your own iOS device.

- Apple Reality Composer [App](https://apps.apple.com/us/app/reality-composer/id1462358802)
- ECA [Diagram](https://github.com/ARpatterns/diagram)
