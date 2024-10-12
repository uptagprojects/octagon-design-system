# Filter Component

The `Filter` component is designed to be used inside a search input to enhance the search functionality by allowing users to filter results based on specific criteria.

## Usage

### Basic Example

```html
<SearchInput>
    <Filter criteria="category" />
    <Filter criteria="date" />
</SearchInput>
```

### Props

- `criteria`: Specifies the filter criteria (e.g., category, date).

### Example with Search Input

```html
<SearchInput placeholder="Search...">
    <Filter criteria="category" />
    <Filter criteria="date" />
    <Filter criteria="status" />
</SearchInput>
```

### Notes

- Ensure that the `Filter` component is placed inside the `SearchInput` component.
- Multiple `Filter` components can be used to provide various filtering options.

## Best Practices

- Use clear and concise criteria names.
- Limit the number of filters to avoid overwhelming the user.
- Provide default filter options to guide the user.

For more detailed information, refer to the [Filter Component Documentation](../filter-component.md).