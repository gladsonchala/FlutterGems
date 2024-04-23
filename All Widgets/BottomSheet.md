## `BottomSheet` Widget

### Overview
The `BottomSheet` widget creates a bottom sheet, which is a material design panel that slides up from the bottom of the screen to reveal additional content or options.

### Usage
```dart
// BottomSheet Widget
// Use the BottomSheet widget to create a bottom sheet.

BottomSheet(
  // Unique Key: Optional key to identify this widget.
  // key: Key('bottom_sheet'),

  // animationController: The animation controller for controlling the bottom sheet's animation.
  animationController: AnimationController(
    vsync: this,
    duration: Duration(milliseconds: 300),
  ),

  // enableDrag: Whether dragging to dismiss the bottom sheet is enabled.
  enableDrag: true,

  // showDragHandle: Whether to show the drag handle at the top of the bottom sheet.
  showDragHandle: true,

  // dragHandleColor: The color of the drag handle.
  dragHandleColor: Colors.grey,

  // dragHandleSize: The size of the drag handle.
  dragHandleSize: Size(50, 5),

  // onDragStart: Callback function triggered when dragging starts.
  onDragStart: (details) {
    // Handle drag start
  },

  // onDragEnd: Callback function triggered when dragging ends.
  onDragEnd: (details, {required isClosing}) {
    // Handle drag end
  },

  // backgroundColor: The background color of the bottom sheet.
  backgroundColor: Colors.white,

  // shadowColor: The color of the shadow cast by the bottom sheet.
  shadowColor: Colors.black,

  // elevation: The elevation of the bottom sheet.
  elevation: 8.0,

  // shape: The shape of the bottom sheet.
  shape: RoundedRectangleBorder(
    borderRadius: BorderRadius.circular(10.0),
  ),

  // clipBehavior: Determines how the bottom sheet's content should be clipped.
  clipBehavior: Clip.antiAlias,

  // constraints: Additional constraints to apply to the bottom sheet.
  constraints: BoxConstraints(
    maxHeight: 300,
  ),

  // onClosing: Callback function triggered when the bottom sheet is closing.
  onClosing: () {
    // Handle closing
  },

  // builder: The builder function to build the content of the bottom sheet.
  builder: (context) {
    return YourBottomSheetContent();
  },
)
```

### Explanation
- Use the `BottomSheet` widget to create a bottom sheet, which slides up from the bottom of the screen.
- Customize the behavior and appearance of the bottom sheet using various properties such as `enableDrag`, `showDragHandle`, `backgroundColor`, `elevation`, etc.
- Specify the animation controller to control the bottom sheet's animation duration and curve.
- The `builder` property is a required callback function that builds the content of the bottom sheet.
- Customize the drag handle's appearance and behavior using properties like `dragHandleColor`, `dragHandleSize`, `onDragStart`, and `onDragEnd`.
- The `onClosing` callback is triggered when the bottom sheet is closing, allowing you to handle any necessary cleanup or state changes.

### Tips
- Use the `ScaffoldState.showBottomSheet` method to create persistent bottom sheets or the `showModalBottomSheet` function for modal bottom sheets.
- Ensure that the content of the bottom sheet is responsive and adapts well to different screen sizes.
- Test the bottom sheet on various devices and orientations to ensure it behaves as expected and looks good in different scenarios.
