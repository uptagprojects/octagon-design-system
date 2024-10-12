# Table Component

The `Table` component is used to display data in a structured tabular format. It is highly customizable and supports various features such as sorting, pagination, and filtering.

## Usage

### Basic Example

```jsx
import { Table } from 'octagon-design-system';

const data = [
    { id: 1, name: 'John Doe', age: 28 },
    { id: 2, name: 'Jane Smith', age: 34 },
];

const columns = [
    { Header: 'ID', accessor: 'id' },
    { Header: 'Name', accessor: 'name' },
    { Header: 'Age', accessor: 'age' },
];

<Table data={data} columns={columns} />
```

### Props

- `data`: An array of objects representing the rows of the table.
- `columns`: An array of objects defining the columns of the table. Each object should have a `Header` and an `accessor`.

### Advanced Features

#### Sorting

To enable sorting, add the `sortable` property to the columns:

```jsx
const columns = [
    { Header: 'ID', accessor: 'id', sortable: true },
    { Header: 'Name', accessor: 'name', sortable: true },
    { Header: 'Age', accessor: 'age', sortable: true },
];
```

#### Pagination

To enable pagination, use the `pagination` prop:

```jsx
<Table data={data} columns={columns} pagination={{ pageSize: 10 }} />
```

#### Filtering

To enable filtering, add the `filterable` property to the columns:

```jsx
const columns = [
    { Header: 'ID', accessor: 'id', filterable: true },
    { Header: 'Name', accessor: 'name', filterable: true },
    { Header: 'Age', accessor: 'age', filterable: true },
];
```

## Conclusion

The `Table` component is a powerful tool for displaying data in a tabular format. By leveraging its various features, you can create highly interactive and user-friendly tables.
