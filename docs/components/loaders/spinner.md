# Spinner Component

The `Spinner` component is used to indicate loading or processing states in your application. It provides a visual cue to users that an action is being performed in the background.

## Usage

To use the `Spinner` component, follow these steps:

1. **Import the Spinner Component:**

    ```javascript
    import { Spinner } from 'octagon-design-system';
    ```

2. **Add the Spinner to Your Component:**

    ```jsx
    function MyComponent() {
      return (
         <div>
            <Spinner />
         </div>
      );
    }
    ```

## Props

The `Spinner` component accepts the following props:

- **size**: Defines the size of the spinner. Possible values are `small`, `medium`, and `large`. Default is `medium`.
- **color**: Sets the color of the spinner. Accepts any valid CSS color value.

### Example

```jsx
<Spinner size="large" color="#3498db" />
```

## Best Practices

- Use the `Spinner` component to indicate loading states for asynchronous operations.
- Ensure the spinner is visible and distinguishable from the background.
- Avoid using multiple spinners on the same page to prevent visual clutter.

## Accessibility

- Provide alternative text for screen readers using `aria-label` or `aria-labelledby`.
- Ensure the spinner is not the only indicator of loading; provide additional context if necessary.

```jsx
<Spinner aria-label="Loading content" />
```

By following these guidelines, you can effectively use the `Spinner` component to enhance the user experience in your application.