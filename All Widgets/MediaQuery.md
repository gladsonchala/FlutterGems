### Overview:
`MediaQuery` is a Flutter widget that provides information about the current media (screen) size and other related information. It allows developers to create responsive layouts by adapting UI components based on the screen size and device orientation.

### Usage:
```dart
MediaQuery(
  // Access media properties using the builder
  builder: (context) {
    // Access media properties here
    final Size screenSize = MediaQuery.of(context).size;
    final EdgeInsets padding = MediaQuery.of(context).padding;
    final bool isLandscape = MediaQuery.of(context).orientation == Orientation.landscape;

    // Return the widget tree with responsive layout
    return Container(
      width: screenSize.width,
      height: screenSize.height - padding.top - padding.bottom,
      child: isLandscape ? _buildLandscapeLayout() : _buildPortraitLayout(),
    );
  },
)
```

### Explanation:
- **builder:** The `builder` property takes a function as an argument, which provides a `BuildContext` parameter. Inside this function, developers can access the media properties using `MediaQuery.of(context)`.

- **MediaQuery Properties:**
  - **size:** Provides the size of the screen (width and height) in logical pixels.
  - **padding:** Provides the padding of the current MediaQuery. This is useful for handling notches, system bars, etc.
  - **orientation:** Returns the orientation of the device, either portrait or landscape.

- **Responsive Layout:**
  - The layout can be adjusted based on the media properties obtained from `MediaQuery`.
  - Developers can conditionally render different UI components or apply different styles based on the screen size or orientation.

### Tips:
- Use `MediaQuery` to create responsive layouts that adapt to different screen sizes and orientations.
- Avoid hardcoding dimensions and use MediaQuery properties instead for better adaptability.
- Be cautious when using MediaQuery in deeply nested widgets to avoid performance issues.

### Example:
In the provided example, `MediaQuery` is used to adjust the layout based on the device orientation. If the device is in landscape mode, `_buildLandscapeLayout()` is called, otherwise `_buildPortraitLayout()` is called.
