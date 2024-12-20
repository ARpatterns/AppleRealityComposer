# Anchored Supplement

![anchored supplement](https://github.com/ARpatterns/declare/raw/main/AnchoredSupplement/docs/images/AnchoredSupplement.jpg)

Provide additional information that is aligned with a detected entity.

* *Use Case* : Anchored Complement
* *Technology Platform* : [Reality Composer](../README.md)
* *Device Type* : handheld
* *Vision System* : world camera

![image](image/anchoredsupplement.gif)

## AR Patterns

**Behavior Patterns**

* [Instant Reaction](https://github.com/ARpatterns/catalog/blob/main/behavioral-patterns/instant-reaction.md): Immediate execution of the superimposition action upon detection of the image as anchorage point.
  * *Event* : on [image](image/emergency_image.png) detection.

**Augmentation Pattern**

* [Anchored Supplement](https://github.com/ARpatterns/catalog/blob/main/augmentation-patterns/anchored-supplement.md): Presentation of 3D content aligned to detected entity for enhancement.
  * *Placed* : on detected image.
  * *Aligned* : with detected image.

## ECA Diagram

| on:start | → | do:detect:image |
| -------- | -- | --------------- |

> '[image](image/emergency_image.png)' detection as anchor👁
>
> | *on:detect* | → | *do:add to AR anchor* |
> | ------------- | -- | ---------------- |
>
>> objects added and aligned to image ➕
>>

## References

- Apple Reality Composer [App](https://apps.apple.com/us/app/reality-composer/id1462358802)
- ECA [Diagram](https://github.com/ARpatterns/diagram)
