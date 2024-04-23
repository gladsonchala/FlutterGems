## `AnimatedCrossFade` Widget
### Use the `AnimatedCrossFade` widget to create a cross-fade animation between two child widgets.

```dart
// AnimatedCrossFade Widget
// Use the AnimatedCrossFade widget to create a cross-fade animation between two child widgets.

AnimatedCrossFade(
  // Unique Key: Optional key to identify this widget.
  // key: Key('animated_cross_fade'),

  // firstChild: The first child widget.
  firstChild: Container(
    width: 200.0,
    height: 200.0,
    color: Colors.blue,
    child: Center(
      child: Text(
        'First Child',
        style: TextStyle(color: Colors.white),
      ),
    ),
  ),

  // secondChild: The second child widget.
  secondChild: Container(
    width: 200.0,
    height: 200.0,
    color: Colors.red,
    child: Center(
      child: Text(
        'Second Child',
        style: TextStyle(color: Colors.white),
      ),
    ),
  ),

  // firstCurve: The curve of the first child's fade-in animation.
  firstCurve: Curves.easeInOut,

  // secondCurve: The curve of the second child's fade-out animation.
  secondCurve: Curves.easeInOut,

  // sizeCurve: The curve of the cross-fade animation's size change.
  sizeCurve: Curves.easeInOut,

  // alignment: The alignment of the cross-fade animation.
  alignment: Alignment.topCenter,

  // crossFadeState: The state of the cross-fade animation.
  crossFadeState: CrossFadeState.showFirst,

  // duration: The duration of the animation.
  duration: Duration(milliseconds: 500),

  // reverseDuration: The duration of the animation when reversing.
  reverseDuration: Duration(milliseconds: 500),

  // layoutBuilder: The builder function used to customize the layout of the children.
  layoutBuilder: (topChild, topChildKey, bottomChild, bottomChildKey) {
    return Stack(
      clipBehavior: Clip.none,
      alignment: Alignment.center,
      children: <Widget>[
        Positioned(
          key: topChildKey,
          child: topChild,
        ),
        Positioned(
          key: bottomChildKey,
          child: bottomChild,
        ),
      ],
    );
  },

  // excludeBottomFocus: Whether to exclude the bottom child from focus when it's not shown.
  excludeBottomFocus: true,
)
```

Additional tips:
- Use `AnimatedCrossFade` to create a smooth cross-fade animation between two child widgets.
- Customize the animation curves for fade-in, fade-out, and size change using the respective curve properties.
- Adjust the alignment of the cross-fade animation using the `alignment` property.
- Specify the duration of the animation using the `duration` property.
- Optionally, you can provide a reverse duration for the animation when it's reversed.
- Customize the layout of the children using the `layoutBuilder` property.
