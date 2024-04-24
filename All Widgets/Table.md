## Table Widget
### Use the Table widget to create a table layout.

```dart
Table(
  // List of table rows
  children: [
    // TableRow 1
    TableRow(
      // List of widgets in the row
      children: [
        // TableCell 1
        TableCell(
          // Widget in the cell
          child: Container(
            alignment: Alignment.center,
            height: 50,
            color: Colors.blue,
            child: Text('Cell 1'),
          ),
        ),
        // TableCell 2
        TableCell(
          // Widget in the cell
          child: Container(
            alignment: Alignment.center,
            height: 50,
            color: Colors.green,
            child: Text('Cell 2'),
          ),
        ),
      ],
    ),
    // TableRow 2
    TableRow(
      // List of widgets in the row
      children: [
        // TableCell 1
        TableCell(
          // Widget in the cell
          child: Container(
            alignment: Alignment.center,
            height: 50,
            color: Colors.orange,
            child: Text('Cell 3'),
          ),
        ),
        // TableCell 2
        TableCell(
          // Widget in the cell
          child: Container(
            alignment: Alignment.center,
            height: 50,
            color: Colors.red,
            child: Text('Cell 4'),
          ),
        ),
      ],
    ),
  ],
);

```

### Properties
- `children`: List of table rows.
- `columnWidths`: Map specifying the width for individual columns.
- `defaultColumnWidth`: Default width for columns that do not have a specified width.
- `textDirection`: Directionality for the table.
- `border`: Border for the table.
- `defaultVerticalAlignment`: Default vertical alignment for cells.
- `textBaseline`: Baseline for aligning text in cells.

### Explanation
- The `Table` widget is used to create a table layout.
- Each row in the table is represented by a `TableRow` widget within the `children` list.
- Within each `TableRow`, individual cells are represented by `TableCell` widgets.
- Cells can contain any widget, allowing for customization of content and appearance.
- The table layout can be customized further using properties like `columnWidths`, `border`, and `defaultVerticalAlignment`.

### Tips
- Use the `Table` widget to create a table layout with rows and cells.
- Customize the appearance of the table using properties like `columnWidths`, `border`, and `defaultVerticalAlignment`.
- Each cell can contain any widget, enabling rich content within the table.
