## DataTable Widget
#### Use the DataTable widget to create a widget describing a data table.

```dart
DataTable(
  // List<DataColumn> columns: A list of DataColumn objects that describes the table's columns.
  columns: [
    DataColumn(label: Text('Name')),
    DataColumn(label: Text('Age')),
    DataColumn(label: Text('Location')),
  ],
  // List<DataRow> rows: A list of DataRow objects that describes the table's rows.
  rows: [
    DataRow(cells: [
      DataCell(Text('John')),
      DataCell(Text('30')),
      DataCell(Text('New York')),
    ]),
    DataRow(cells: [
      DataCell(Text('Emily')),
      DataCell(Text('25')),
      DataCell(Text('Los Angeles')),
    ]),
    DataRow(cells: [
      DataCell(Text('Michael')),
      DataCell(Text('35')),
      DataCell(Text('Chicago')),
    ]),
  ],
  // int? sortColumnIndex: The index of the column that is currently sorted.
  sortColumnIndex: 0,
  // bool sortAscending: Whether the sort order is ascending or descending.
  sortAscending: true,
  // bool showCheckboxColumn: Whether to display the checkbox column at the beginning of the table.
  showCheckboxColumn: false,
);

```

### Properties
- `columns`: A list of DataColumn objects that describes the table's columns.
- `rows`: A list of DataRow objects that describes the table's rows.
- `sortColumnIndex`: The index of the column that is currently sorted.
- `sortAscending`: Whether the sort order is ascending or descending.
- `showCheckboxColumn`: Whether to display the checkbox column at the beginning of the table.

### Explanation
- The `DataTable` widget is used to create a table with rows and columns of data.
- Each column in the table is represented by a `DataColumn`, and each row is represented by a `DataRow`.
- The `columns` property is a list of `DataColumn` objects, specifying the table's columns.
- The `rows` property is a list of `DataRow` objects, specifying the table's rows.
- If sorting is enabled, you can specify the index of the column that is currently sorted using `sortColumnIndex`, and the sort order using `sortAscending`.
- Set `showCheckboxColumn` to true if you want to display a checkbox column at the beginning of the table, typically for selecting rows.

### Tips
- Use the `DataColumn` widget to define the header of each column.
- Use the `DataRow` widget to define each row of data.
- Customize the appearance and behavior of the table using properties such as `dataRowHeight`, `headingRowColor`, `headingRowHeight`, etc.
