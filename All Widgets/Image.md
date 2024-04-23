## `Image` Widget

#### Overview
The `Image` widget displays an image.

### Usage
```dart
// Image Widget
// Use the Image widget to display an image.

Image(
  // required ImageProvider<Object> image: The image to display.
  image: AssetImage('assets/image.png'),

  // frameBuilder: Widget Function(BuildContext, Widget, int?, bool)? to build the widget that represents loading progress.
  // frameBuilder: (context, child, frame, wasSynchronouslyLoaded) {
  //   if (frame == null) return CircularProgressIndicator();
  //   return child;
  // },

  // loadingBuilder: Widget Function(BuildContext, Widget, ImageChunkEvent?)? to build the widget that represents loading.
  // loadingBuilder: (context, child, loadingProgress) {
  //   if (loadingProgress == null) return child;
  //   return CircularProgressIndicator(value: loadingProgress.expectedTotalBytes != null ? loadingProgress.cumulativeBytesLoaded / loadingProgress.expectedTotalBytes! : null);
  // },

  // errorBuilder: Widget Function(BuildContext, Object, StackTrace?)? to build the widget that represents an error.
  // errorBuilder: (context, error, stackTrace) => Text('Error: $error'),

  // String? semanticLabel: A semantic description of the image.
  semanticLabel: 'Image',

  // bool excludeFromSemantics: Whether the image should be excluded from semantics.
  excludeFromSemantics: false,

  // double? width: The width of the image.
  width: 100,

  // double? height: The height of the image.
  height: 100,

  // Color? color: The color to apply to the image.
  // color: Colors.red,

  // Animation<double>? opacity: The opacity of the image.
  // opacity: AlwaysStoppedAnimation(0.5),

  // BlendMode? colorBlendMode: The blend mode to apply to the image.
  // colorBlendMode: BlendMode.modulate,

  // BoxFit? fit: How the image should be inscribed into the space allocated during layout.
  fit: BoxFit.cover,

  // AlignmentGeometry alignment: How the image should be aligned within its container.
  alignment: Alignment.center,

  // ImageRepeat repeat: How the image should be repeated if it does not fill its layout bounds.
  // repeat: ImageRepeat.repeat,

  // Rect? centerSlice: The rectangle to use for centering and scaling the image within the destination rectangle.
  // centerSlice: Rect.fromLTRB(20, 20, 100, 100),

  // bool matchTextDirection: Whether to paint the image in the direction of the [TextDirection].
  // matchTextDirection: true,

  // bool gaplessPlayback: Whether to continue showing the old image (true) or briefly show nothing (false) when the image provider changes.
  gaplessPlayback: false,

  // bool isAntiAlias: Whether to apply anti-aliasing to the image.
  isAntiAlias: false,

  // FilterQuality filterQuality: The filter quality for the image.
  // filterQuality: FilterQuality.high,
)
```

#### Explanation
- The `Image` widget displays an image.
- Specify the image to display using the `image` property, which requires an `ImageProvider<Object>`.
- Use `frameBuilder`, `loadingBuilder`, and `errorBuilder` to customize the loading, progress, and error representations of the image respectively.
- Provide a semantic label for the image using the `semanticLabel` property.
- Set `excludeFromSemantics` to `true` to exclude the image from semantics.
- Specify the width and height of the image using the `width` and `height` properties respectively.
- Apply a color to the image using the `color` property.
- Control the opacity of the image with the `opacity` property.
- Apply a blend mode to the image using the `colorBlendMode` property.
- Define how the image should be inscribed into the space allocated during layout using the `fit` property.
- Align the image within its container using the `alignment` property.
- Control how the image should be repeated if it does not fill its layout bounds with the `repeat` property.
- Use `centerSlice` to specify a rectangle to use for centering and scaling the image within the destination rectangle.
- Set `matchTextDirection` to `true` to paint the image in the direction of the `TextDirection`.
- Specify whether to continue showing the old image (`true`) or briefly show nothing (`false`) when the image provider changes using `gaplessPlayback`.
- Apply anti-aliasing to the image using the `isAntiAlias` property.
- Set the filter quality for the image using `filterQuality`.

### Tips
- Use `Image.asset` for images from the asset bundle and `Image.network` for images from the network.
- Customize the loading, progress, and error representations of the image using the builder properties.
- Adjust the image size, color, alignment, and other properties to fit your UI requirements.
- Consider the image's aspect ratio, fit, and repeat mode to ensure proper display within your layout.
