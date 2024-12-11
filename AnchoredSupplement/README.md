# Anchored Supplement

![anchored supplement](https://github.com/ARpatterns/declare/raw/main/AnchoredSupplement/docs/images/AnchoredSupplement.jpg)

Provide additional information that is aligned with a detected entity.

* *Use Case* : Anchored Complement
* *Technology Platform* : [Reality Composer](../README.md)
* *Device Type* : handheld
* *Vision System* : world camera

## AR Patterns

**Behavior Patterns**

* [Instant Reaction](https://github.com/ARpatterns/catalog/blob/main/behavioral-patterns/instant-reaction.md): Immediate execution of the superimposition action
  * *Event* : on [image](AnchoredSupplement/emergencypicture.jpg) detection
* [Conditional Reaction](https://github.com/ARpatterns/catalog/blob/main/behavioral-patterns/conditional-reaction.md): remove superimposed object when no longer visible.

**Augmentation Pattern**

* [Anchored Supplement](https://github.com/ARpatterns/catalog/blob/main/augmentation-patterns/anchored-supplement.md): Presentation of 3D content aligned to detected entity for enhancement.
  * *Placed* : on detected image.
  * *Aligned* : with detected image.
