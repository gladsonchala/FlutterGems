```dart
// FilledButton Widget
// Use the FilledButton widget to create a Material Design filled button.

FilledButton(
  // required void Function()? onPressed: The callback function when the button is pressed.
  onPressed: () {
    // Add your button press logic here
  },
  // Widget? child: The child widget inside the button.
  child: Text('Filled Button'),
  // ButtonStyle? style: The style of the button.
  style: FilledButton.styleFrom(
    // Color? backgroundColor: The background color of the button.
    backgroundColor: Colors.blue,
    // ShapeBorder? shape: The shape of the button.
    shape: RoundedRectangleBorder(
      borderRadius: BorderRadius.circular(8.0),
    ),
    // EdgeInsetsGeometry? padding: The padding of the button.
    padding: EdgeInsets.symmetric(
      vertical: 12.0,
      horizontal: 24.0,
    ),
  ),
)

```

### Properties
- `onPressed`: The callback function when the button is pressed.
- `child`: The child widget inside the button.
- `style`: The style of the button.

### Explanation
- The `FilledButton` widget creates a Material Design filled button.
- You can define the button's appearance and behavior using properties like `onPressed`, `child`, and `style`.
- The `style` property allows you to customize various aspects of the button's appearance, such as its background color, shape, padding, etc.

### Tips
- Use the `FilledButton` widget for primary actions or prominent buttons in your app.
- Customize the button's appearance and behavior to match your app's design language and user experience.
- Ensure that the `onPressed` callback function is provided to make the button interactive.
