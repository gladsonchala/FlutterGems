## `MaterialButton` Widget

#### Overview
The `MaterialButton` widget creates a Material Design button.

### Usage
```dart
// MaterialButton Widget
// Use the MaterialButton widget to create a Material Design button.

MaterialButton(
  // required void Function()? onPressed: Callback when the button is pressed.
  onPressed: () {
    // Add your onPressed functionality here
  },

  // void Function()? onLongPress: Callback when the button is long-pressed.
  // onLongPress: () {
  //   print('Long press');
  // },

  // void Function(bool)? onHighlightChanged: Callback when the button's highlight state changes.
  // onHighlightChanged: (isHighlighted) {
  //   print('Highlighted: $isHighlighted');
  // },

  // ButtonTextTheme? textTheme: The text theme to use for the button.
  // textTheme: ButtonTextTheme.primary,

  // Color? textColor: The color of the button's text.
  // textColor: Colors.white,

  // Color? disabledTextColor: The color of the button's text when disabled.
  // disabledTextColor: Colors.grey,

  // Color? color: The button's background color.
  // color: Colors.blue,

  // Color? disabledColor: The button's background color when disabled.
  // disabledColor: Colors.grey,

  // Color? focusColor: The color of the button's background when focused.
  // focusColor: Colors.blueAccent,

  // Color? hoverColor: The color of the button's background when hovered.
  // hoverColor: Colors.lightBlueAccent,

  // Color? highlightColor: The color of the button's background when pressed.
  // highlightColor: Colors.blue[700],

  // Color? splashColor: The color of the splash effect when tapped.
  // splashColor: Colors.blue[800],

  // double? elevation: The elevation of the button.
  // elevation: 4,

  // double? focusElevation: The elevation of the button when focused.
  // focusElevation: 6,

  // double? hoverElevation: The elevation of the button when hovered.
  // hoverElevation: 6,

  // double? highlightElevation: The elevation of the button when pressed.
  // highlightElevation: 8,

  // double? disabledElevation: The elevation of the button when disabled.
  // disabledElevation: 0,

  // EdgeInsetsGeometry? padding: The padding of the button's content.
  // padding: EdgeInsets.symmetric(vertical: 12, horizontal: 24),

  // ShapeBorder? shape: The shape of the button.
  // shape: RoundedRectangleBorder(
  //   borderRadius: BorderRadius.circular(10),
  // ),

  // FocusNode? focusNode: The focus node to use for the button.
  // focusNode: FocusNode(),

  // bool autofocus: Whether the button should be autofocus.
  autofocus: false,

  // MaterialTapTargetSize? materialTapTargetSize: The target size of the button.
  // materialTapTargetSize: MaterialTapTargetSize.shrinkWrap,

  // Duration? animationDuration: The duration of the button's animations.
  // animationDuration: Duration(milliseconds: 200),

  // double? minWidth: The minimum width of the button.
  // minWidth: 150,

  // double? height: The height of the button.
  // height: 48,

  // bool enableFeedback: Whether to enable feedback on press.
  enableFeedback: true,

  // Widget? child: The child widget of the button.
  child: Text('Material Button'),
)
```

#### Explanation
- The `MaterialButton` widget creates a Material Design button.
- Define the `onPressed` callback to execute when the button is pressed.
- Optionally, use `onLongPress` to handle long-press events.
- Utilize `onHighlightChanged` to react to the button's highlight state changes.
- Customize the button's appearance and behavior using various properties such as `textTheme`, `textColor`, `disabledTextColor`, `color`, `disabledColor`, `focusColor`, `hoverColor`, `highlightColor`, `splashColor`, `elevation`, `focusElevation`, `hoverElevation`, `highlightElevation`, `disabledElevation`, `padding`, `shape`, `focusNode`, `autofocus`, `materialTapTargetSize`, `animationDuration`, `minWidth`, `height`, and `enableFeedback`.

### Tips
- Use `MaterialButton` for basic interactions in your app, such as submitting a form or triggering an action.
- Customize the appearance of the button, including colors, elevation, and shape, to match your app's design and branding.
- Ensure consistent padding and text styles across buttons for a cohesive look and feel.
- Test the button's behavior on different devices and screen sizes to ensure responsiveness and accessibility.
