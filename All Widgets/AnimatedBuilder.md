## `AnimatedBuilder` Widget
### Use the `AnimatedBuilder` widget to create an animated builder.

```dart
// AnimatedBuilder Widget
// Use the AnimatedBuilder widget to create an animated builder.

AnimatedBuilder(
  // Unique Key: Optional key to identify this widget.
  // key: Key('animated_builder'),

  // animation: The listenable animation that triggers the builder function.
  animation: animationController, // Provide your animation controller here

  // builder: The builder function that returns the widget to be animated.
  builder: (context, child) {
    return Container(
      width: animation.value * 100, // Animated width
      height: animation.value * 100, // Animated height
      color: Colors.blue,
      child: Center(
        child: Text(
          'Animated Container',
          style: TextStyle(color: Colors.white),
        ),
      ),
    );
  },

  // child: The child widget, if any.
  child: YourChildWidget(),
)
```

Additional tips:
- Use `AnimatedBuilder` to create widgets that animate based on a `Listenable` object, such as an `AnimationController`.
- The `builder` function is called every time the animation value changes. It returns the widget to be animated.
- Inside the builder function, you can access the current value of the animation and use it to update the properties of the animated widget.
- Provide the animation controller or other listenable object in the `animation` parameter.
- You can optionally include a `child` widget that doesn't rebuild with the animation but is part of the widget tree.
