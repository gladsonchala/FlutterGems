## `AnimatedSize` Widget
### Use the `AnimatedSize` widget to animate its size to match that of its child.

```dart
// AnimatedSize Widget
// Use the AnimatedSize widget to animate its size to match that of its child.

AnimatedSize(
  // Unique Key: Optional key to identify this widget.
  // key: Key('animated_size'),

  // child: The child widget whose size will be animated.
  child: YourChildWidget(),

  // alignment: The alignment of the child within the AnimatedSize.
  alignment: Alignment.center,

  // curve: The curve to apply when animating the size.
  curve: Curves.easeInOut,

  // duration: The duration of the animation.
  duration: Duration(milliseconds: 500),

  // reverseDuration: The duration of the animation when reversing.
  reverseDuration: Duration(milliseconds: 500),

  // clipBehavior: The clipping behavior of the widget.
  clipBehavior: Clip.hardEdge,

  // onEnd: A callback function called when the animation ends.
  onEnd: () {
    // Perform actions after the animation ends.
  },
)
```

Additional tips:
- Use `AnimatedSize` to animate its size to match that of its child.
- Customize the alignment of the child within the `AnimatedSize` using the `alignment` property.
- Customize the animation curve using the `curve` property, and set the duration of the animation using the `duration` property.
- Set `reverseDuration` to control the duration of the animation when reversing.
- Specify the clipping behavior of the widget using the `clipBehavior` property.
- You can provide an `onEnd` callback to perform actions after the animation completes.
