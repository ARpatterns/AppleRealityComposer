# Capture Twin

![image](image/Capture_twin.png)

A *captured twin* is a digital replica of a physical object, created using data from sensors or cameras. In Reality Composer, this process, known as  *3D Capture*, involves taking multiple images of an object from different angles and using *photogrammetry* to combine them into a 3D model. These models can then be imported into Reality Composer projects, allowing users to interact with them in AR environments.

* _Use Case_: Virtual Object Replica
* _Technology Platform_: [Reality Composer](../README.md)
* _Device Type_: handheld
* _Vision System_: world camera

## 3D Object Capture

<img src="image/3D_capture.jpg" width="420"/>

Apple's Reality Composer uses the "Object Capture" feature to create realistic 3D models from photographs. The process involves positioning the object in good lighting, adjusting the capture frame and capturing images by moving your device around the object in multiple loops at different angles.

<img src="image/Interface.png" width="270"/>

The app processes these images to generate a detailed 3D model, which can be viewed, manipulated, or used in AR. Models can be saved as USDZ files for cross-platform compatibility or reprocessed on a Mac for enhanced quality.

### Capture Workflow

__Preparation Steps__
* _Lighting and Positioning_: Ensure the object is placed in a well-lit environment with even lighting to minimize shadows.
* _Framing the Object_: Adjust the capture frame to fully enclose the object and ensure all details are visible.

__Capture Process__
* _Multi-Angle Imaging_: Move around the object slowly, capturing images from multiple angles to provide complete coverage for accurate 3D reconstruction.
* _Real-Time Feedback_: Follow on-screen guides to refine your positioning and ensure all areas of the object are adequately scanned.

__Post-Capture Tips__
* Optionally reprocess the captured data on a Mac for higher-quality results.

<img src="image/Aromat_twin.png" width="270"/>

Presentation of captured twin next to the original.

### AR Patterns

__Behavior Pattern__

* [Instant Reaction](https://github.com/ARpatterns/catalog/blob/main/behavioral-patterns/instant-reaction.md):

![image](image/Bottle.png)
