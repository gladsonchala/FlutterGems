## `AnimatedPhysicalModel` Widget
### Use the `AnimatedPhysicalModel` widget to animate the properties of a `PhysicalModel`.

```dart
// AnimatedPhysicalModel Widget
// Use the AnimatedPhysicalModel widget to animate the properties of a PhysicalModel.

AnimatedPhysicalModel(
  // Unique Key: Optional key to identify this widget.
  // key: Key('animated_physical_model'),

  // child: The child widget contained by the physical model.
  child: YourChildWidget(),

  // shape: The shape of the physical model.
  shape: BoxShape.rectangle,

  // clipBehavior: The clipping behavior of the physical model.
  clipBehavior: Clip.none,

  // borderRadius: The border radius of the physical model.
  borderRadius: BorderRadius.zero,

  // elevation: The elevation of the physical model.
  elevation: 10.0,

  // color: The color of the physical model.
  color: Colors.blue,

  // animateColor: Whether to animate the color of the physical model.
  animateColor: true,

  // shadowColor: The shadow color of the physical model.
  shadowColor: Colors.black,

  // animateShadowColor: Whether to animate the shadow color of the physical model.
  animateShadowColor: true,

  // curve: The curve to apply when animating the properties.
  curve: Curves.easeInOut,

  // duration: The duration of the animation.
  duration: Duration(milliseconds: 500),

  // onEnd: A callback function called when the animation ends.
  onEnd: () {
    // Perform actions after the animation ends.
  },
)
```

Additional tips:
- Use `AnimatedPhysicalModel` to animate the properties of a `PhysicalModel`.
- Customize the shape, clipping behavior, border radius, elevation, color, and shadow color of the physical model.
- Set `animateColor` to true to animate the color of the physical model.
- Set `animateShadowColor` to true to animate the shadow color of the physical model.
- Customize the animation curve using the `curve` property, and set the duration of the animation using the `duration` property.
- You can provide an `onEnd` callback to perform actions after the animation completes.
