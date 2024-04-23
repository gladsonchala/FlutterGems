## `Container` Widget

#### Overview
The `Container` widget combines common painting, positioning, and sizing widgets.

### Usage
```dart
// Container Widget
// Use the Container widget to create a combination of common painting, positioning, and sizing widgets.

Container(
  // Unique Key: Optional key to identify this widget.
  // key: Key('container'),

  // alignment: AlignmentGeometry to align the child within the container.
  alignment: Alignment.center,

  // padding: EdgeInsetsGeometry to apply padding around the child.
  padding: EdgeInsets.all(16.0),

  // color: Color to fill the background of the container.
  color: Colors.blue,

  // decoration: Decoration to apply to the container's background.
  // To supply a decoration with a color, use decoration: BoxDecoration(color: color).
  // decoration: BoxDecoration(
  //   color: Colors.blue,
  //   borderRadius: BorderRadius.circular(8.0),
  // ),

  // foregroundDecoration: Decoration to apply to the container's foreground.
  // foregroundDecoration: BoxDecoration(
  //   border: Border.all(color: Colors.red, width: 2.0),
  // ),

  // width: double to set the width of the container.
  width: 200.0,

  // height: double to set the height of the container.
  height: 200.0,

  // constraints: BoxConstraints to apply additional constraints to the container's size.
  // constraints: BoxConstraints(minWidth: 100.0, minHeight: 100.0, maxWidth: 300.0, maxHeight: 300.0),

  // margin: EdgeInsetsGeometry to apply margin around the container.
  margin: EdgeInsets.all(8.0),

  // transform: Matrix4 to apply a 3D transformation to the container.
  // transform: Matrix4.rotationZ(0.1),

  // transformAlignment: AlignmentGeometry to align the transform.
  // transformAlignment: Alignment.center,

  // child: Widget to be placed inside the container.
  child: Text('Hello World'),

  // clipBehavior: Clip to determine how the container's contents should be clipped.
  clipBehavior: Clip.none,
)
```

#### Explanation
- The `Container` widget combines common painting, positioning, and sizing widgets.
- Use the `alignment` property to align the child within the container.
- Apply padding around the child using the `padding` property.
- Set the background color of the container using the `color` property.
- Alternatively, apply a decoration to the container's background using the `decoration` property. To use both `color` and `decoration`, provide the color within the `BoxDecoration`.
- Apply a decoration to the container's foreground using the `foregroundDecoration` property.
- Use `width` and `height` to set the size of the container.
- Apply additional constraints to the container's size using the `constraints` property.
- Add margin around the container using the `margin` property.
- Apply a 3D transformation to the container using the `transform` property.
- Align the transformation using the `transformAlignment` property.
- Place a child widget inside the container using the `child` property.
- Determine how the container's contents should be clipped using the `clipBehavior` property.

### Tips
- Use the `Container` widget as a versatile layout element to customize appearance and layout.
- Combine properties like `color`, `decoration`, `padding`, and `alignment` to create visually appealing designs.
- Apply transformations to the container using the `transform` property for advanced visual effects.
- Use the `margin` property to add space around the container within its parent.
