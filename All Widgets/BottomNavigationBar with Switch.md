Using a normal switch statement without a controller to change pages of `BottomNavigationBar`:

```dart
import 'package:flutter/material.dart';

class MyBottomNavigationBarWidget extends StatefulWidget {
  @override
  _MyBottomNavigationBarWidgetState createState() =>
      _MyBottomNavigationBarWidgetState();
}

class _MyBottomNavigationBarWidgetState
    extends State<MyBottomNavigationBarWidget> {
  int _selectedIndex = 0;
  Widget _currentPage = Center(child: Text('Home Page'));

  void _onItemTapped(int index) {
    setState(() {
      _selectedIndex = index;
      switch (_selectedIndex) {
        case 0:
          _currentPage = Center(child: Text('Home Page'));
          break;
        case 1:
          _currentPage = Center(child: Text('Search Page'));
          break;
        case 2:
          _currentPage = Center(child: Text('Profile Page'));
          break;
      }
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('BottomNavigationBar Example'),
      ),
      body: _currentPage,
      bottomNavigationBar: BottomNavigationBar(
        items: const <BottomNavigationBarItem>[
          BottomNavigationBarItem(
            icon: Icon(Icons.home),
            label: 'Home',
          ),
          BottomNavigationBarItem(
            icon: Icon(Icons.search),
            label: 'Search',
          ),
          BottomNavigationBarItem(
            icon: Icon(Icons.person),
            label: 'Profile',
          ),
        ],
        currentIndex: _selectedIndex,
        selectedItemColor: Colors.blue,
        onTap: _onItemTapped,
      ),
    );
  }
}
```

In this version, the `_onItemTapped` function updates the `_selectedIndex` variable and then uses a switch statement to update the `_currentPage` variable with the appropriate page widget based on the selected index. The body of the Scaffold displays the `_currentPage` widget, which changes dynamically when a tab is tapped.
