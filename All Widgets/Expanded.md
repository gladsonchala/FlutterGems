## `Expanded` Widget
#### Use the `Expanded` widget to make a child widget fill the available space along the main axis of a Row, Column, or Flex.

```dart
Row(
  children: [
    Container(
      color: Colors.blue,
      height: 50,
      width: 50,
    ),
    // Expanded widget expands to fill the remaining space
    Expanded(
      // int flex: The flex factor to use for this child.
      flex: 2,
      child: Container(
        color: Colors.red,
        height: 50,
      ),
    ),
    Container(
      color: Colors.blue,
      height: 50,
      width: 50,
    ),
  ],
);

```

### Properties
- `flex`: The flex factor to use for this child. This determines how much space this child should occupy relative to the other children.

### Explanation
- The `Expanded` widget is used within a `Row`, `Column`, or `Flex` to make its child fill the available space along the main axis.
- In the example, there are three containers wrapped in a row. The middle container is wrapped in an `Expanded` widget with a `flex` of 2, so it takes up twice as much space as the other containers.
- The `flex` property determines how much space the child should occupy relative to other children. In this example, the middle container with `flex: 2` takes up twice as much space as the other containers.

### Tips
- Use the `Expanded` widget when you want a child widget to fill the available space along the main axis of a row, column, or flex.
- The `flex` property allows you to control how much space the child should occupy relative to other children in the same parent widget.
