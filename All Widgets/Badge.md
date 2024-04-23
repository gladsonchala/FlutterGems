## `Badge` Widget

### Overview
The `Badge` widget allows you to add a badge on top of another widget. It's commonly used to indicate new or unread items, notifications, or any other status.

### Usage
```dart
// Badge Widget
// Use the Badge widget to create a badge that stacks label on top of child.

Badge(
  // Unique Key: Optional key to identify this widget.
  // key: Key('badge'),

  // backgroundColor: The background color of the badge.
  backgroundColor: Colors.red,

  // textColor: The text color of the label.
  textColor: Colors.white,

  // smallSize: The size of the badge when applied to a small widget.
  smallSize: 20,

  // largeSize: The size of the badge when applied to a large widget.
  largeSize: 30,

  // textStyle: The text style of the label.
  textStyle: TextStyle(fontSize: 12, fontWeight: FontWeight.bold),

  // padding: The padding around the label.
  padding: EdgeInsets.all(4),

  // alignment: The alignment of the badge.
  alignment: Alignment.topRight,

  // offset: The offset to adjust the position of the badge.
  offset: Offset(-5, 5),

  // label: The widget to be displayed as the label.
  label: Text('New'),

  // isLabelVisible: Whether the label is visible or not.
  isLabelVisible: true,

  // child: The child widget to apply the badge to.
  child: YourChildWidget(),
)
```

### Explanation
- Use the `Badge` widget to stack a label on top of another widget, creating a badge effect.
- Customize the appearance of the badge using properties like `backgroundColor`, `textColor`, `textStyle`, and `padding`.
- Specify the size of the badge using `smallSize` and `largeSize` properties, which are used for different widget sizes.
- Adjust the alignment and position of the badge using `alignment` and `offset` properties.
- If `label` is null, only a filled circle is displayed; otherwise, the label is displayed within a stadium-shaped area.

### Tips
- Experiment with different colors, sizes, and text styles to create badges that match your app's design.
- You can use badges to indicate various states, such as new items, notifications, or errors.
- Consider making the label optional to use the badge purely for visual decoration without any text.
- Test the badge with different widgets to ensure it looks good and remains visible across different screen sizes and orientations.
