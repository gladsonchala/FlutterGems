### ClipRect Widget

#### Overview
The `ClipRect` widget creates a rectangular clip.

#### Usage
```dart
// ClipRect Widget
// Use the ClipRect widget to create a rectangular clip.

ClipRect(
  // Unique Key: Optional key to identify this widget.
  // key: Key('clip_rect'),

  // clipper: CustomClipper<Rect> to specify a custom clip rectangle.
  // clipper: CustomClipper<Rect>,

  // clipBehavior: Determines how to clip the child.
  // Use Clip.hardEdge for a rectangular clip.
  // clipBehavior: Clip.hardEdge,

  // child: The widget to be clipped with the rectangular clip.
  child: Container(
    width: 100,
    height: 100,
    color: Colors.blue,
  ),
)
```

#### Explanation
- The `ClipRect` widget creates a rectangular clip.
- Use the `clipper` property to specify a custom clip rectangle using a `CustomClipper<Rect>`.
- Set the `clipBehavior` property to determine how to clip the child. Use `Clip.hardEdge` for a rectangular clip.
- Wrap the child widget you want to clip with the `ClipRect` widget.

#### Tips
- The `ClipRect` widget is useful for creating rectangular clips for child widgets.
- You can specify a custom clip rectangle by providing a `CustomClipper<Rect>` to the `clipper` property.
- Adjust the child widget's size to control the area affected by the rectangular clip.
