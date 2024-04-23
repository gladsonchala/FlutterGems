## `Chip` Widget

### Overview
The `Chip` widget creates a Material Design chip.

### Usage
```dart
// Chip Widget
// Use the Chip widget to create a Material Design chip.

Chip(
  // Unique Key: Optional key to identify this widget.
  // key: Key('chip'),

  // avatar: An optional leading widget (typically an avatar).
  avatar: CircleAvatar(
    backgroundColor: Colors.blue,
    child: Text('A'),
  ),

  // label: The primary content of the chip.
  label: Text('Chip'),

  // labelStyle: The style of the label text.
  labelStyle: TextStyle(color: Colors.black),

  // labelPadding: The padding around the label.
  labelPadding: EdgeInsets.all(8.0),

  // deleteIcon: An optional widget to display at the end of the chip (typically a delete icon).
  deleteIcon: Icon(Icons.close),

  // onDeleted: Callback function called when the delete icon is tapped.
  onDeleted: () {
    // Handle delete action here
  },

  // deleteIconColor: The color of the delete icon.
  deleteIconColor: Colors.red,

  // deleteButtonTooltipMessage: The tooltip message to show when hovering over the delete icon.
  deleteButtonTooltipMessage: 'Delete',

  // side: The border side of the chip.
  side: BorderSide(color: Colors.black),

  // shape: The shape of the chip.
  shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(20)),

  // clipBehavior: The clipping behavior of the chip.
  clipBehavior: Clip.none,

  // autofocus: Whether the chip should be focused automatically.
  autofocus: true,

  // color: The background color of the chip.
  color: MaterialStateProperty.all(Colors.grey),

  // backgroundColor: The background color of the chip.
  backgroundColor: Colors.grey[200],

  // padding: The padding around the chip.
  padding: EdgeInsets.all(8.0),

  // visualDensity: The visual density of the chip.
  visualDensity: VisualDensity.standard,

  // materialTapTargetSize: The size of the tap target.
  materialTapTargetSize: MaterialTapTargetSize.shrinkWrap,

  // elevation: The elevation of the chip.
  elevation: 2.0,

  // shadowColor: The shadow color of the chip.
  shadowColor: Colors.grey,

  // surfaceTintColor: The tint color of the chip's surface.
  surfaceTintColor: Colors.white,

  // iconTheme: The theme data for the icons within the chip.
  iconTheme: IconThemeData(color: Colors.blue),
)
```

### Explanation
- The `Chip` widget creates a Material Design chip.
- The `avatar` property allows you to add an optional leading widget, typically an avatar.
- The `label` property is the primary content of the chip.
- The `deleteIcon` property allows you to add an optional widget to display at the end of the chip, typically a delete icon.
- The `onDeleted` callback is called when the delete icon is tapped.
- Customize the appearance of the chip using properties like `labelStyle`, `labelPadding`, `deleteIconColor`, `deleteButtonTooltipMessage`, `side`, `shape`, `clipBehavior`, `autofocus`, `color`, `backgroundColor`, `padding`, `visualDensity`, `materialTapTargetSize`, `elevation`, `shadowColor`, `surfaceTintColor`, and `iconTheme`.

### Tips
- Use the chip widget to represent simple pieces of information, actions, or attributes.
- Customize the appearance of the chip to match the design of your application.
- Utilize the `onDeleted` callback to handle delete actions when the delete icon is tapped.
