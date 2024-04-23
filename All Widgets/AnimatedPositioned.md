## `AnimatedPositioned` Widget
### Use the `AnimatedPositioned` widget to animate its position implicitly.

```dart
// AnimatedPositioned Widget
// Use the AnimatedPositioned widget to animate its position implicitly.

AnimatedPositioned(
  // Unique Key: Optional key to identify this widget.
  // key: Key('animated_positioned'),

  // child: The child widget whose position will be animated.
  child: YourChildWidget(),

  // left: The left edge of the positioned child.
  left: 100.0,

  // top: The top edge of the positioned child.
  top: 100.0,

  // right: The right edge of the positioned child.
  // If both left and right are non-null, width is ignored.
  //right: 100.0,

  // bottom: The bottom edge of the positioned child.
  // If both top and bottom are non-null, height is ignored.
  //bottom: 100.0,

  // width: The width of the positioned child.
  //width: 100.0,

  // height: The height of the positioned child.
  //height: 100.0,

  // curve: The curve to apply when animating the position.
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
- Use `AnimatedPositioned` to animate the position of its child implicitly.
- Specify the position of the child using properties like `left`, `top`, `right`, `bottom`.
- At least one value out of `left`, `right`, and `width` must be null, and similarly, at least one value out of `top`, `bottom`, and `height` must be null.
- Customize the animation curve using the `curve` property, and set the duration of the animation using the `duration` property.
- You can provide an `onEnd` callback to perform actions after the animation completes.
