Creating a responsive design in Flutter involves using `MediaQuery`, `LayoutBuilder`, and `Flex widgets` to adapt to different screen sizes. Here's an example:

```dart
import 'package:flutter/material.dart';

class ResponsiveWidget extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('Responsive Design Example'),
      ),
      body: Center(
        child: LayoutBuilder(
          builder: (BuildContext context, BoxConstraints constraints) {
            if (constraints.maxWidth < 600) {
              return _buildMobileLayout();
            } else {
              return _buildDesktopLayout();
            }
          },
        ),
      ),
    );
  }

  Widget _buildMobileLayout() {
    return Column(
      mainAxisAlignment: MainAxisAlignment.center,
      children: [
        Text(
          'Welcome to Mobile View',
          style: TextStyle(fontSize: 20),
        ),
        SizedBox(height: 20),
        _buildButton('Mobile Button'),
      ],
    );
  }

  Widget _buildDesktopLayout() {
    return Row(
      mainAxisAlignment: MainAxisAlignment.center,
      children: [
        Expanded(
          flex: 1,
          child: Text(
            'Welcome to Desktop View',
            style: TextStyle(fontSize: 20),
          ),
        ),
        Expanded(
          flex: 1,
          child: Padding(
            padding: const EdgeInsets.all(8.0),
            child: _buildButton('Desktop Button 1'),
          ),
        ),
        Expanded(
          flex: 1,
          child: Padding(
            padding: const EdgeInsets.all(8.0),
            child: _buildButton('Desktop Button 2'),
          ),
        ),
      ],
    );
  }

  Widget _buildButton(String label) {
    return ElevatedButton(
      onPressed: () {
        // Action when button is pressed
        print('$label pressed.');
      },
      child: Text(label),
    );
  }
}
```

Explanation:
- This example demonstrates a responsive design where the layout changes based on the screen width.
- The `LayoutBuilder` widget is used to check the constraints of the parent widget (screen).
- If the screen width is less than 600 (indicating a mobile view), `_buildMobileLayout()` is called, which displays elements vertically.
- If the screen width is 600 or more (indicating a desktop view), `_buildDesktopLayout()` is called, which displays elements horizontally.
- Each layout method returns a different widget structure tailored to the screen size.
- The `_buildButton` method creates a button widget with a given label.

You can further adjust the constraints and layouts based on your specific requirements and breakpoints.
