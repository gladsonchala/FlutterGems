## `Actions` Widget
### Use the `Actions` widget to create a widget that dispatches specific actions to its child widgets.

```dart
// Actions Widget
// Use the Actions widget to create a widget that dispatches specific actions to its child widgets.

Actions(
  // Unique Key: Optional key to identify this widget.
  // key: Key('actions'),

  // dispatcher: The action dispatcher used to dispatch actions.
  dispatcher: ActionDispatcher(),

  // actions: A map of actions to be dispatched.
  actions: {
    YourActionType1: CallbackAction((Intent intent) {
      // Define the action to be performed for YourActionType1.
    }),
    YourActionType2: CallbackAction((Intent intent) {
      // Define the action to be performed for YourActionType2.
    }),
    // Add more actions as needed.
  },

  // child: The widget subtree to which this Actions widget applies.
  child: YourWidget(),
)
```

Additional tips:
- Use `Actions` to dispatch specific actions to its child widgets.
- Define the actions and their corresponding callbacks in the `actions` map.
- Ensure that each action is an instance of `Action<Intent>` or a subclass of it.
- Wrap the widgets that need to respond to the dispatched actions within the `Actions` widget.
