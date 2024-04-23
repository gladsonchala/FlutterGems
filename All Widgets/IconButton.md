## `IconButton` Widget

#### Overview
The `IconButton` widget creates an icon button.

### Usage
```dart
// IconButton Widget
// Use the IconButton widget to create an icon button.

IconButton(
  // double? iconSize: The size of the icon.
  iconSize: 24,

  // VisualDensity? visualDensity: The visual density for the button.
  // visualDensity: VisualDensity.compact,

  // EdgeInsetsGeometry? padding: The padding for the button's hit region.
  // padding: EdgeInsets.all(8),

  // AlignmentGeometry? alignment: The alignment of the icon.
  // alignment: Alignment.center,

  // double? splashRadius: The splash radius of the button.
  // splashRadius: 24,

  // Color? color: The color of the button's icon.
  // color: Colors.blue,

  // Color? focusColor: The color for the button's focus highlight.
  // focusColor: Colors.red,

  // Color? hoverColor: The color for the button's hover highlight.
  // hoverColor: Colors.green,

  // Color? highlightColor: The color for the button's press highlight.
  // highlightColor: Colors.orange,

  // Color? splashColor: The color for the button's splash effect.
  // splashColor: Colors.yellow,

  // Color? disabledColor: The color for the button when it is disabled.
  // disabledColor: Colors.grey,

  // required void Function()? onPressed: The function to call when the button is pressed.
  onPressed: () {
    // Add your onPressed functionality here
  },

  // MouseCursor? mouseCursor: The mouse cursor to use for the button.
  // mouseCursor: MouseCursor.defer,

  // FocusNode? focusNode: The focus node to use for the button.
  // focusNode: FocusNode(),

  // bool autofocus: Whether the button should be autofocus.
  autofocus: false,

  // String? tooltip: The tooltip to show when the button is hovered over.
  // tooltip: 'Click me',

  // bool? enableFeedback: Whether to provide haptic feedback when the button is pressed.
  // enableFeedback: true,

  // BoxConstraints? constraints: Additional constraints for the button.
  // constraints: BoxConstraints.tightFor(width: 48, height: 48),

  // ButtonStyle? style: The style to apply to the button.
  // style: ButtonStyle(
  //   backgroundColor: MaterialStateProperty.all(Colors.blue),
  //   foregroundColor: MaterialStateProperty.all(Colors.white),
  //   padding: MaterialStateProperty.all(EdgeInsets.all(8)),
  // ),

  // bool? isSelected: Whether the button is selected.
  // isSelected: false,

  // Widget? selectedIcon: The icon to display when the button is selected.
  // selectedIcon: Icon(Icons.check),

  // required Widget icon: The icon to display on the button.
  icon: Icon(Icons.add),
)
```

#### Explanation
- The `IconButton` widget creates an icon button.
- Set the size of the icon with the `iconSize` property.
- Adjust the visual density of the button using the `visualDensity` property.
- Define the padding for the button's hit region with the `padding` property.
- Align the icon within the button using the `alignment` property.
- Specify the splash radius of the button with the `splashRadius` property.
- Set the color of the button's icon with the `color` property.
- Customize the colors for focus, hover, highlight, splash effects, and disabled state using the respective properties.
- Provide a function to call when the button is pressed with the `onPressed` property.
- Specify the mouse cursor to use for the button with the `mouseCursor` property.
- Set the focus node for the button using the `focusNode` property.
- Determine whether the button should be autofocus using the `autofocus` property.
- Define a tooltip to show when the button is hovered over with the `tooltip` property.
- Enable or disable haptic feedback when the button is pressed using the `enableFeedback` property.
- Apply additional constraints to the button using the `constraints` property.
- Customize the button's style using the `style` property, which accepts a `ButtonStyle`.
- Set `isSelected` to `true` if the button is selected, and provide a `selectedIcon` to display when selected.
- Specify the icon to display on the button using the required `icon` property.

### Tips
- Use `IconButton` for clickable icons, commonly found in app bars or as action buttons.
- Customize the appearance and behavior of the button using various properties such as colors, sizes, and padding.
- Provide meaningful tooltips for better user experience.
- Utilize haptic feedback to give users tactile confirmation of button presses.
- Ensure proper accessibility by setting appropriate visual and semantic properties for the button.
