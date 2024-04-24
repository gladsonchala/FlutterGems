## TabBar Widget
#### Use the TabBar widget to create a Material Design primary tab bar.

```dart
DefaultTabController(
  length: 3, // Number of tabs
  child: TabBar(
    // List of tabs
    tabs: [
      Tab(text: 'Tab 1'),
      Tab(text: 'Tab 2'),
      Tab(text: 'Tab 3'),
    ],
    // Tab controller to coordinate tabs with their content
    // If not provided, there must be a DefaultTabController ancestor
    controller: TabController(length: 3, vsync: this),
    // Set to true to allow scrolling when there are many tabs
    isScrollable: true,
    // Style for the indicator below the selected tab
    indicatorColor: Colors.blue,
    // Weight of the indicator line
    indicatorWeight: 4.0,
    // Padding around the indicator
    indicatorPadding: EdgeInsets.symmetric(horizontal: 16.0),
    // Color for the label text of the selected tab
    labelColor: Colors.black,
    // Style for the label text of the selected tab
    labelStyle: TextStyle(fontSize: 16, fontWeight: FontWeight.bold),
    // Padding around the label text
    labelPadding: EdgeInsets.symmetric(vertical: 8.0),
    // Color for the label text of unselected tabs
    unselectedLabelColor: Colors.grey,
    // Style for the label text of unselected tabs
    unselectedLabelStyle: TextStyle(fontSize: 16),
    // Called when a tab is tapped
    onTap: (index) {
      // Handle tab selection
      print('Selected tab: $index');
    },
  ),
);

```

### Properties
- `tabs`: List of widgets representing the tabs.
- `controller`: Tab controller to coordinate tabs with their content.
- `isScrollable`: Set to true to allow scrolling when there are many tabs.
- `indicatorColor`: Color of the indicator below the selected tab.
- `indicatorWeight`: Weight of the indicator line.
- `indicatorPadding`: Padding around the indicator.
- `labelColor`: Color for the label text of the selected tab.
- `labelStyle`: Style for the label text of the selected tab.
- `labelPadding`: Padding around the label text.
- `unselectedLabelColor`: Color for the label text of unselected tabs.
- `unselectedLabelStyle`: Style for the label text of unselected tabs.
- `onTap`: Callback function called when a tab is tapped.

### Explanation
- The `TabBar` widget is used to create a Material Design primary tab bar.
- It is typically used as a child of a `DefaultTabController`.
- Each tab is represented by a `Tab` widget within the `tabs` list.
- The `controller` property is used to coordinate tabs with their content.
- Various properties like `indicatorColor`, `labelColor`, `labelStyle`, etc., can be used to customize the appearance of the tab bar.

### Tips
- Use the `TabBar` widget within a `DefaultTabController` to create a tab bar with tabs.
- Customize the appearance of the tab bar using properties like `indicatorColor`, `labelColor`, `labelStyle`, etc.
- Handle tab selection using the `onTap` callback function.
