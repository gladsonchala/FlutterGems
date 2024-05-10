## `BottomNavigationBar` Widget

### Overview
The `BottomNavigationBar` widget creates a bottom navigation bar, which is typically used as the `bottomNavigationBar` argument of a `Scaffold`.

### Usage
```dart
// BottomNavigationBar Widget
// Use the BottomNavigationBar widget to create a bottom navigation bar.

BottomNavigationBar(
  // Unique Key: Optional key to identify this widget.
  // key: Key('bottom_navigation_bar'),

  // items: The list of navigation items to display.
  items: [
    BottomNavigationBarItem(
      icon: Icon(Icons.home),
      label: 'Home',
    ),
    BottomNavigationBarItem(
      icon: Icon(Icons.search),
      label: 'Search',
    ),
    BottomNavigationBarItem(
      icon: Icon(Icons.notifications),
      label: 'Notifications',
    ),
    BottomNavigationBarItem(
      icon: Icon(Icons.person),
      label: 'Profile',
    ),
  ],

  // onTap: Callback function triggered when a navigation item is tapped.
  onTap: (index) {
    // Handle tap
  },

  // currentIndex: The index of the currently selected item.
  currentIndex: 0,

  // backgroundColor: The background color of the navigation bar.
  backgroundColor: Colors.white,

  // selectedItemColor: The color of the selected item.
  selectedItemColor: Colors.blue,

  // unselectedItemColor: The color of the unselected items.
  unselectedItemColor: Colors.grey,

  // showSelectedLabels: Whether to show labels for the selected items.
  showSelectedLabels: true,

  // showUnselectedLabels: Whether to show labels for the unselected items.
  showUnselectedLabels: true,
)
```

### Explanation
- Use the `BottomNavigationBar` widget to create a bottom navigation bar with multiple navigation items.
- Customize the appearance and behavior of the navigation bar using various properties such as `items`, `selectedItemColor`, `unselectedItemColor`, `showSelectedLabels`, etc.
- The `items` property is a list of `BottomNavigationBarItem` objects, each representing a navigation item with an icon and a label.
- The `onTap` callback function is triggered when a navigation item is tapped, allowing you to handle navigation logic.
- Set the `currentIndex` property to specify the index of the currently selected item.
- You can customize the appearance of the navigation bar using properties like `backgroundColor`, `elevation`, `iconSize`, etc.
- Use the `showSelectedLabels` and `showUnselectedLabels` properties to control whether labels are displayed for selected and unselected items.

### Tips
- Ensure that the length of the `items` list is at least two, and each item's icon and label are not null.
- Test the navigation bar on different devices and screen sizes to ensure it looks good and behaves as expected.
- Consider using a `Scaffold` with a `BottomNavigationBar` for a complete app layout with navigation.
