## `ElevatedButton` Widget

#### Overview
The `ElevatedButton` widget creates a Material Design elevated button.

### Usage
```dart
// ElevatedButton Widget
// Use the ElevatedButton widget to create a raised button.

ElevatedButton(
  // required void Function()? onPressed: Callback when the button is pressed.
  onPressed: () {
    // Add your onPressed functionality here
  },

  // void Function()? onLongPress: Callback when the button is long-pressed.
  // onLongPress: () {
  //   print('Long press');
  // },

  // void Function(bool)? onHover: Callback when the button's hover state changes.
  // onHover: (isHovering) {
  //   print('Hovering: $isHovering');
  // },

  // void Function(bool)? onFocusChange: Callback when the button's focus state changes.
  // onFocusChange: (hasFocus) {
  //   print('Focus: $hasFocus');
  // },

  // ButtonStyle? style: The style to apply to the button.
  // style: ButtonStyle(
  //   backgroundColor: MaterialStateProperty.all(Colors.blue),
  //   foregroundColor: MaterialStateProperty.all(Colors.white),
  //   padding: MaterialStateProperty.all(EdgeInsets.all(16)),
  // ),

  // FocusNode? focusNode: The focus node to use for the button.
  // focusNode: FocusNode(),

  // bool autofocus: Whether the button should be autofocus.
  autofocus: false,

  // Clip clipBehavior: The clip behavior to use for the button.
  clipBehavior: Clip.none,

  // required Widget? child: The child widget of the button.
  child: Text('Elevated Button'),
)
```

#### Explanation
- The `ElevatedButton` widget creates a raised button.
- Define the `onPressed` callback to execute when the button is pressed.
- Optionally, use `onLongPress` to handle long-press events.
- Utilize `onHover` to react to hover state changes.
- Use `onFocusChange` to respond to focus state changes.
- Customize the button's appearance and behavior using the `style` property, which accepts a `ButtonStyle`.
- Specify a `focusNode` to manage the button's focus behavior.
- Set `autofocus` to `true` if the button should be autofocus.
- Define the clip behavior using `clipBehavior`.
- Provide a child widget for the button using the required `child` property.

### Tips
- Use `ElevatedButton` for primary actions in your app, such as submitting forms or initiating important actions.
- Customize the button's appearance, including colors, padding, and shape, using the `style` property.
- Ensure accessibility by providing meaningful labels and handling focus and hover states appropriately.
- Test the button's behavior on different devices and screen sizes to ensure consistent user experience across platforms.
