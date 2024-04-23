## `Center` Widget

### Overview
The `Center` widget creates a container that centers its child both horizontally and vertically within itself.

### Usage
```dart
// Center Widget
// Use the Center widget to center its child horizontally and vertically.

Center(
  // Unique Key: Optional key to identify this widget.
  // key: Key('center'),

  // widthFactor: Factor to multiply the child's width by.
  // widthFactor: 1.0,

  // heightFactor: Factor to multiply the child's height by.
  // heightFactor: 1.0,

  // child: The child widget to be centered.
  child: Container(
    width: 100.0,
    height: 100.0,
    color: Colors.blue,
    child: Text('Centered Content'),
  ),
)
```

### Explanation
- Use the `Center` widget to center its child both horizontally and vertically within itself.
- You can optionally specify `widthFactor` and `heightFactor` to scale the child's width and height, respectively.
- The `child` property is the widget to be centered.

### Tips
- Use the `Center` widget to ensure that its child is visually centered within its parent widget.
- Adjust the `widthFactor` and `heightFactor` if you want the child to occupy a fraction of the available space.
- The `Center` widget is useful for creating layouts where you need to position content at the center of the screen or within another container.
