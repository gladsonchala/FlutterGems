## `Text` Widget

#### Overview
The `Text` widget creates a text element.

### Usage
```dart
// Text Widget
// Use the Text widget to display text.

Text(
  // String data: The text to display.
  'Hello, Flutter!',

  // Unique Key: Optional key to identify this widget.
  // key: Key('text'),

  // style: TextStyle to customize the text's appearance.
  style: TextStyle(
    // fontFamily: String to specify the font family.
    // fontFamily: 'Roboto',

    // fontSize: double to set the size of the text.
    // fontSize: 18.0,

    // fontWeight: FontWeight to specify the font weight.
    // fontWeight: FontWeight.bold,

    // fontStyle: FontStyle to specify the font style.
    // fontStyle: FontStyle.italic,

    // color: Color to set the text color.
    // color: Colors.black,

    // letterSpacing: double to adjust the space between letters.
    // letterSpacing: 1.0,

    // wordSpacing: double to adjust the space between words.
    // wordSpacing: 2.0,

    // decoration: TextDecoration to add decoration to the text.
    // decoration: TextDecoration.underline,

    // decorationColor: Color to set the color of the decoration.
    // decorationColor: Colors.blue,

    // decorationStyle: TextDecorationStyle to set the style of the decoration.
    // decorationStyle: TextDecorationStyle.dashed,

    // decorationThickness: double to set the thickness of the decoration.
    // decorationThickness: 2.0,

    // backgroundColor: Color to set the background color behind the text.
    // backgroundColor: Colors.yellow,

    // shadows: List of Shadows to add shadows to the text.
    // shadows: [Shadow(color: Colors.grey, offset: Offset(2, 2), blurRadius: 3)],
  ),

  // textAlign: TextAlign to specify the text alignment.
  textAlign: TextAlign.center,

  // textDirection: TextDirection to specify the text direction.
  // textDirection: TextDirection.ltr,

  // softWrap: bool to specify whether the text should wrap.
  // softWrap: true,

  // overflow: TextOverflow to specify how overflowing text should be handled.
  // overflow: TextOverflow.ellipsis,

  // maxLines: int to specify the maximum number of lines to display.
  // maxLines: 2,

  // semanticsLabel: String to specify a semantic label for accessibility.
  // semanticsLabel: 'Hello',

  // selectionColor: Color to set the color of the text selection highlight.
  // selectionColor: Colors.blue,

)
```

#### Explanation
- The `Text` widget displays text.
- Use the `style` property to customize the appearance of the text.
- Specify the text alignment using the `textAlign` property.
- Optionally, set the text direction using the `textDirection` property.
- Use `softWrap` to allow the text to wrap if it exceeds the available space.
- Control how overflowing text is handled with the `overflow` property.
- Limit the number of lines displayed using the `maxLines` property.
- Provide a semantic label for accessibility using the `semanticsLabel` property.
- Customize the text selection highlight color with the `selectionColor` property.

### Tips
- Customize the appearance of text using properties like `fontSize`, `fontWeight`, `color`, `decoration`, and more within the `TextStyle`.
- Use `textAlign` to ensure your text is aligned correctly within its container.
- Set `softWrap` to `true` if you want long texts to wrap to the next line.
- Control how overflowing text is displayed with the `overflow` property.
- Use `maxLines` to limit the number of lines displayed, especially in constrained spaces.
