## `Radio` Widget

#### Overview
The `Radio` widget creates a Material Design radio button.

### Usage
```dart
// Radio Widget
// Use the Radio widget to create a Material Design radio button.

Radio(
  // required dynamic value: The value that represents this radio button.
  value: 'value',

  // required dynamic groupValue: The currently selected value.
  groupValue: 'selectedValue',

  // required void Function(dynamic)? onChanged: Callback when the radio button is changed.
  onChanged: (newValue) {
    // Add your onChanged functionality here
  },

  // bool toggleable: Whether this radio button can be toggled.
  // toggleable: true,

  // Color? activeColor: The color to use when this radio button is selected.
  // activeColor: Colors.blue,

  // Color? focusColor: The color to use when this radio button has the input focus.
  // focusColor: Colors.blueAccent,

  // Color? hoverColor: The color to use when this radio button is hovered over.
  // hoverColor: Colors.lightBlueAccent,

  // double? splashRadius: The splash radius of the radio button when pressed.
  // splashRadius: 20,

  // MaterialTapTargetSize? materialTapTargetSize: The target size of the radio button.
  // materialTapTargetSize: MaterialTapTargetSize.shrinkWrap,

  // VisualDensity? visualDensity: The visual density of the radio button.
  // visualDensity: VisualDensity.compact,

  // FocusNode? focusNode: The focus node for the radio button.
  // focusNode: FocusNode(),

  // bool autofocus: Whether this radio button should be autofocus.
  autofocus: false,
)
```

#### Explanation
- The `Radio` widget creates a Material Design radio button.
- Specify the `value` of the radio button, which represents this option.
- `groupValue` indicates the currently selected value among all radio buttons in the same group.
- `onChanged` is called when the radio button is selected, allowing you to update the `groupValue`.
- Optionally, set `toggleable` to true if the radio button can be toggled to deselect.
- Customize appearance with properties like `activeColor`, `focusColor`, `hoverColor`, `splashRadius`, `materialTapTargetSize`, `visualDensity`, `focusNode`, and `autofocus`.

### Tips
- Use `Radio` buttons when you have a set of mutually exclusive options and only one can be selected.
- Ensure that the `groupValue` and `value` properties are set correctly to manage the selected state.
- Customize the appearance of the radio button to match your app's design using properties like `activeColor`, `focusColor`, and `hoverColor`.
- Test the radio button behavior with different input devices and screen sizes to ensure usability and accessibility.
