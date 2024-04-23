## `AnimatedWidget` Widget
### Use the `AnimatedWidget` widget to rebuild when the given listenable changes.

```dart
// AnimatedWidget Widget
// Use the AnimatedWidget widget to rebuild when the given listenable changes.

AnimatedWidget(
  // Unique Key: Optional key to identify this widget.
  // key: Key('animated_widget'),

  // listenable: The Listenable object to listen for changes.
  listenable: yourListenableObject,

  // builder: A builder function that returns a widget based on the current value of the listenable.
  builder: (BuildContext context, Widget? child) {
    // Your widget tree based on the current value of the listenable.
    return YourAnimatedWidget();
  },
)
```

Additional tips:
- Use `AnimatedWidget` to rebuild when the given listenable changes.
- Provide the `listenable` argument with the Listenable object to listen for changes.
- Implement the `builder` function to return a widget based on the current value of the listenable.
- The widget returned by the builder will be rebuilt whenever the value of the listenable changes.
