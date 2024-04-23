```dart
// Drawer Widget
// Use the Drawer widget to create a Material Design drawer.

Drawer(
  // Color? backgroundColor: The background color of the drawer.
  backgroundColor: Colors.white,
  // double? elevation: The elevation of the drawer.
  elevation: 16.0,
  // Color? shadowColor: The color of the shadow below the drawer.
  shadowColor: Colors.black,
  // ShapeBorder? shape: The shape of the drawer.
  shape: RoundedRectangleBorder(
    borderRadius: BorderRadius.only(
      topRight: Radius.circular(20.0),
      bottomRight: Radius.circular(20.0),
    ),
  ),
  // double? width: The width of the drawer.
  width: 250.0,
  // Widget? child: The content of the drawer.
  child: ListView(
    padding: EdgeInsets.zero,
    children: [
      DrawerHeader(
        decoration: BoxDecoration(
          color: Colors.blue,
        ),
        child: Text(
          'Drawer Header',
          style: TextStyle(
            color: Colors.white,
            fontSize: 24,
          ),
        ),
      ),
      ListTile(
        title: Text('Item 1'),
        onTap: () {
          // Handle item 1 tap
        },
      ),
      ListTile(
        title: Text('Item 2'),
        onTap: () {
          // Handle item 2 tap
        },
      ),
      ListTile(
        title: Text('Item 3'),
        onTap: () {
          // Handle item 3 tap
        },
      ),
    ],
  ),
)

```

### Properties
- `backgroundColor`: The background color of the drawer.
- `elevation`: The elevation of the drawer.
- `shadowColor`: The color of the shadow below the drawer.
- `shape`: The shape of the drawer.
- `width`: The width of the drawer.
- `child`: The content of the drawer.

### Explanation
- The `Drawer` widget creates a Material Design drawer.
- It is typically used in the `Scaffold.drawer` property.
- You can customize the appearance of the drawer using properties like `backgroundColor`, `elevation`, `shadowColor`, `shape`, and `width`.
- The content of the drawer is defined using the `child` property, usually a `ListView` containing `ListTile` widgets.
- The `DrawerHeader` widget can be used to add a header to the drawer.

### Tips
- Use the `Drawer` widget to provide navigation options or additional content in your app.
- Customize the appearance of the drawer to match your app's design language.
- Add interactive items like `ListTile` widgets inside the drawer for navigation or actions.
