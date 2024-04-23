## `Checkbox` Widget

### Overview
The `Checkbox` widget creates a Material Design checkbox.

### Usage
```dart
// Checkbox Widget
// Use the Checkbox widget to create a Material Design checkbox.

Checkbox(
  // Unique Key: Optional key to identify this widget.
  // key: Key('checkbox'),

  // value: Whether the checkbox is checked.
  value: isChecked,

  // tristate: Whether the checkbox can have three states: checked, unchecked, or indeterminate.
  tristate: false,

  // onChanged: Callback function called when the checkbox value changes.
  onChanged: (newValue) {
    setState(() {
      isChecked = newValue!;
    });
  },

  // activeColor: The color of the checkbox when it's checked.
  activeColor: Colors.green,

  // fillColor: The color of the checkbox when it's checked, focused, or hovered.
  fillColor: MaterialStateProperty.all(Colors.blue),

  // checkColor: The color of the checkmark inside the checkbox.
  checkColor: Colors.white,

  // focusColor: The color of the checkbox when it's focused.
  focusColor: Colors.red,

  // hoverColor: The color of the checkbox when it's hovered.
  hoverColor: Colors.yellow,

  // overlayColor: The color of the checkbox's splash overlay.
  overlayColor: MaterialStateProperty.all(Colors.orange),

  // splashRadius: The radius of the splash effect when the checkbox is tapped.
  splashRadius: 20.0,

  // materialTapTargetSize: The size of the tap target.
  materialTapTargetSize: MaterialTapTargetSize.shrinkWrap,

  // visualDensity: The visual density of the checkbox.
  visualDensity: VisualDensity.standard,

  // focusNode: The focus node for managing the focus state of the checkbox.
  focusNode: FocusNode(),

  // autofocus: Whether the checkbox should be focused automatically.
  autofocus: true,

  // shape: The shape of the checkbox.
  shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(10)),

  // side: The border side of the checkbox.
  side: BorderSide(color: Colors.black),

  // isError: Whether the checkbox is in an error state.
  isError: false,

  // semanticLabel: A description of the checkbox for screen readers.
  semanticLabel: 'This is a checkbox',
)
```

### Explanation
- The `Checkbox` widget creates a Material Design checkbox.
- The `value` property determines whether the checkbox is checked. The `onChanged` callback is called when the value of the checkbox changes.
- Most widgets that use a checkbox will listen for the `onChanged` callback and rebuild the checkbox with a new value to update the visual appearance of the checkbox.
- The `tristate` property allows the checkbox to have three states: checked, unchecked, or indeterminate. It can only be used when `value` is nullable.
- The appearance of the checkbox can be customized using properties like `activeColor`, `fillColor`, `checkColor`, `focusColor`, `hoverColor`, `overlayColor`, `splashRadius`, `materialTapTargetSize`, `visualDensity`, `focusNode`, `autofocus`, `shape`, `side`, `isError`, and `semanticLabel`.

### Tips
- Customize the appearance of the checkbox to match the theme of your application.
- Ensure that the `onChanged` callback updates the state of the checkbox correctly to reflect its new value.
- Use the `autofocus` property carefully, as it automatically focuses the checkbox when the widget is initialized.
