# Search Input Component

The Search Input component is used to allow users to enter search queries. This document explains the proper usage of the Search Input component in the Octagon Design System.

## Usage

### Basic Example

```html
<SearchInput placeholder="Search..." />
```

### Props

- `placeholder` (string): The placeholder text displayed in the input field.
- `value` (string): The current value of the search input.
- `onChange` (function): Callback function called when the input value changes.

### Example with Props

```html
<SearchInput 
    placeholder="Search for items..." 
    value={searchValue} 
    onChange={handleSearchChange} 
/>
```

### Accessibility

Ensure that the search input is accessible by providing appropriate `aria-label` or `aria-labelledby` attributes.

```html
<SearchInput 
    placeholder="Search..." 
    aria-label="Search through site content" 
/>
```

## Best Practices

- Use clear and concise placeholder text.
- Ensure the search input is easily identifiable.
- Provide feedback for search results.

## Conclusion

The Search Input component is a versatile and essential part of the Octagon Design System, enabling users to perform search operations efficiently.
