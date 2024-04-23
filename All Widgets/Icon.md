## `Icon` Widget

### Overview
The `Icon` widget is used to display graphical icons based on `IconData`.

### Usage
```dart
// Icon Widget
// Use the Icon widget to display graphical icons based on IconData.

Icon(
  // IconData icon: The icon to display.
  Icons.star,
  // double size: The size of the icon.
  size: 24,
  // Color color: The color of the icon.
  color: Colors.blue,
)
```

### Properties
- `icon`: The IconData representing the icon to display.
- `size`: The size of the icon.
- `color`: The color of the icon.
- `semanticLabel`: A label for the icon used by screen readers.

### Explanation
- The `Icon` widget is used to display graphical icons based on `IconData`.
- It accepts an `icon` parameter of type `IconData`, which determines which icon to display.
- The `size` property defines the size of the icon, and the `color` property sets the color of the icon.
- Optionally, you can provide a `semanticLabel` for accessibility purposes, which is used by screen readers to describe the icon to users with visual impairments.

### Tips
- Use `Icon` widgets to add visual indicators or actions to your UI.
- Icons can be customized by adjusting the `size` and `color` properties.
- Choose appropriate icons that convey meaning effectively in your application.
- Provide `semanticLabel` for icons that convey important information for accessibility purposes.
