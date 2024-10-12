# Link Component

The `Link` component is used to create hyperlinks to navigate between different pages or sections within your application. It provides a consistent styling and behavior for all links in your design system.

## Usage

### Basic Example

```jsx
import { Link } from 'octagon-design-system';

const Example = () => (
    <div>
        <Link href="https://example.com">Visit Example</Link>
    </div>
);
```

### Props

- `href` (string): The URL that the hyperlink points to. This is a required prop.
- `target` (string): Specifies where to open the linked document. Common values are `_self`, `_blank`, `_parent`, and `_top`.
- `rel` (string): Specifies the relationship between the current document and the linked document. Common values are `noopener` and `noreferrer`.

### Styling

The `Link` component can be styled using CSS classes or inline styles. It inherits styles from the parent component and can be customized to fit the design requirements.

### Accessibility

Ensure that the `Link` component is accessible by providing meaningful text within the link. Avoid using generic text like "click here" or "read more".

### Example with Target and Rel

```jsx
import { Link } from 'octagon-design-system';

const Example = () => (
    <div>
        <Link href="https://example.com" target="_blank" rel="noopener noreferrer">
            Visit Example
        </Link>
    </div>
);
```

## Best Practices

- Use descriptive link text to improve accessibility.
- Ensure that links are easily distinguishable from regular text.
- Avoid using links for actions that do not involve navigation.

By following these guidelines, you can ensure that the `Link` component is used effectively and consistently throughout your application.