## `AbsorbPointer` Widget
### Use the `AbsorbPointer` widget to create a widget that absorbs pointers during hit testing (not clickable set of widgets).

```dart
// AbsorbPointer Widget
// Use the AbsorbPointer widget to create a widget that absorbs pointers during hit testing (not clickable set of widgets).

AbsorbPointer(
  // Unique Key: Optional key to identify this widget.
  // key: Key('absorb_pointer'),

  // absorbing: Whether this widget absorbs pointers during hit testing.
  // If true, this widget prevents its subtree from receiving pointer events.
  absorbing: true,

  // ignoringSemantics: Whether the semantics of this widget should be ignored.
  // If true, this widget will be ignored by the semantics layer.
  ignoringSemantics: true,

  // child: The widget below this widget in the tree.
  child: ElevatedButton(
    onPressed: () {
      // This button is not clickable when wrapped by AbsorbPointer.
    },
    child: Text('Click Me'),
  ),
)
```

Additional tips:
- Use `AbsorbPointer` when you want to prevent user interaction with a subtree of widgets.
- It can be useful for scenarios where you want to disable a portion of the UI temporarily or conditionally.
- Remember that `AbsorbPointer` prevents pointer events but doesn't affect the layout or appearance of its child widget.
