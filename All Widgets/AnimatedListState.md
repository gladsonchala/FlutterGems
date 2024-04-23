## `AnimatedListState` Class
### Use the `AnimatedListState` class to interact with an `AnimatedList`.

```dart
// AnimatedListState
// Use the AnimatedListState class to interact with an AnimatedList.

AnimatedListState _listState = GlobalKey<AnimatedListState>();

// Access the state methods like insertItem, removeItem, etc.
_listState.insertItem(index);
_listState.removeItem(index, (context, animation) => YourRemovedItemWidget());

// Get the current items count
int itemCount = _listState.getItemCount();

// Get the current items
List<Widget> items = _listState.getItems();
```

Additional tips:
- Use `AnimatedListState` to interact with an `AnimatedList`.
- You can access the state of an `AnimatedList` using a `GlobalKey<AnimatedListState>`.
- Call methods like `insertItem` and `removeItem` to animate items being inserted or removed from the list.
- Retrieve the current items count using `getItemCount`.
- Retrieve the current items using `getItems`.
- Make sure to use the `setState` method when modifying the state of the `AnimatedList`.
