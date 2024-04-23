## `ListTile` Widget

### Overview
The `ListTile` widget is used to create a list item in Flutter, commonly used in lists and menus.

### Usage
```dart
// ListTile Widget
// Use the ListTile widget to create a list item.

ListTile(
  // Widget? leading: A widget to display before the title.
  leading: Icon(Icons.person),
  // Widget? title: The primary content of the list tile.
  title: Text('John Doe'),
  // Widget? subtitle: Additional content displayed below the title.
  subtitle: Text('johndoe@example.com'),
  // Widget? trailing: A widget to display after the title.
  trailing: Icon(Icons.arrow_forward),
  // bool isThreeLine: Whether this list tile is intended to display three lines of text.
  isThreeLine: true,
  // bool? dense: Whether this list tile is vertically dense.
  dense: true,
  // Color? tileColor: The background color of the list tile.
  tileColor: Colors.grey[200],
  // void Function()? onTap: Called when the list tile is tapped.
  onTap: () {
    // Handle onTap event
  },
)
```

### Properties
- `leading`: A widget to display before the title.
- `title`: The primary content of the list tile.
- `subtitle`: Additional content displayed below the title.
- `trailing`: A widget to display after the title.
- `isThreeLine`: Whether this list tile is intended to display three lines of text.
- `dense`: Whether this list tile is vertically dense.
- `tileColor`: The background color of the list tile.
- `onTap`: Called when the list tile is tapped.

### Explanation
- The `ListTile` widget creates a list item with optional leading, trailing, title, and subtitle widgets.
- It is commonly used in lists and menus to display items with additional details.
- The `leading` widget is displayed before the title, such as an icon or avatar.
- The `title` widget is the primary content of the list tile, typically a text widget.
- The `subtitle` widget is additional content displayed below the title.
- The `trailing` widget is displayed after the title, such as an icon or arrow.
- The `isThreeLine` property is used to indicate whether the list tile is intended to display three lines of text.
- The `dense` property determines whether the list tile is vertically dense.
- The `tileColor` property sets the background color of the list tile.
- The `onTap` property is called when the list tile is tapped.

### Tips
- Use `ListTile` widgets to create list items with leading, trailing, title, and subtitle content.
- Customize the appearance of the list tile using properties like `tileColor`, `dense`, and `isThreeLine`.
- Handle tap events using the `onTap` property to make list items interactive.
- Experiment with different combinations of leading, trailing, title, and subtitle widgets to create visually appealing list items.
