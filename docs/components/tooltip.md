# Tooltip Component

The Tooltip component is used to display informative text when users hover over, focus on, or tap an element.

## Usage

### Basic Example

To use the Tooltip component, wrap the target element with the `Tooltip` component and provide the text you want to display as a prop.

```jsx
import { Tooltip } from 'octagon-design-system';

function Example() {
    return (
        <Tooltip text="This is a tooltip">
            <button>Hover over me</button>
        </Tooltip>
    );
}
```

### Props

- `text` (string): The text to display inside the tooltip. This prop is required.
- `position` (string): The position of the tooltip relative to the target element. Possible values are `top`, `right`, `bottom`, and `left`. Default is `top`.

### Advanced Example

You can customize the position of the tooltip using the `position` prop.

```jsx
import { Tooltip } from 'octagon-design-system';

function AdvancedExample() {
    return (
        <Tooltip text="Tooltip on the right" position="right">
            <button>Hover over me</button>
        </Tooltip>
    );
}
```

### Accessibility

Ensure that the Tooltip component is accessible by providing appropriate ARIA attributes and keyboard interactions.

```jsx
import { Tooltip } from 'octagon-design-system';

function AccessibleExample() {
    return (
        <Tooltip text="Accessible tooltip" aria-label="Tooltip information">
            <button>Focus on me</button>
        </Tooltip>
    );
}
```

## Best Practices

- Keep the tooltip text concise and informative.
- Use tooltips sparingly to avoid overwhelming users.
- Ensure tooltips are accessible to all users, including those using keyboard navigation and screen readers.

For more information, refer to the [Octagon Design System documentation](https://octagon-design-system.com/docs/components/tooltip).
