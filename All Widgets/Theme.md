## Theme Widget
### Use the Theme widget to apply a theme to its child widget.

```dart
Theme(
  // ThemeData to apply
  data: ThemeData(
    // Define the theme properties here
    primaryColor: Colors.blue,
    accentColor: Colors.green,
    // Add more theme properties as needed
  ),
  // Child widget
  child: YourWidget(),
);

```

### Properties
- `data`: The `ThemeData` to apply to the child widget.
- `child`: The child widget to which the theme is applied.

### Explanation
- The `Theme` widget applies a theme to its child widget, allowing you to customize the appearance of the child and its descendants.
- The `data` property of the `Theme` widget is set to a `ThemeData` object containing the desired theme properties.
- You can customize various aspects of the theme, such as colors, typography, and shapes, by providing values to the `ThemeData` constructor.
- Any descendant widget of the `Theme` widget will inherit the theme properties defined in the `data`.

### Tips
- Use the `Theme` widget to apply consistent styling across your app.
- Customize the theme properties in the `ThemeData` object to match your app's design language.
- Encapsulate parts of your UI that share common styling within `Theme` widgets to maintain a consistent look and feel.
