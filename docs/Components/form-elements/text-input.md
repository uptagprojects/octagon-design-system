# TextInput Component

The `TextInput` component is a versatile input field used for collecting user input in the form of text. It is commonly used in forms and can be customized to fit various use cases.

## Usage

To use the `TextInput` component, import it into your project and include it in your JSX:

```jsx
import { TextInput } from 'octagon-ui';

function MyForm() {
    return (
        <form>
            <TextInput label="username" name="username" placeholder="Enter your username" />
        </form>
    );
}
```

## Props

The `TextInput` component accepts any of the `<input />` props, plus the following:

- `label` (string): The label for the input field.
- `icon` (string): An icon that will be shown on the left.
- `size` ("small", "medium", "large"): The size of the input. Defaults to `medium`.
- `errorMessage` (string): An input error to be shown at the bottom.
- `hideLabel` (boolean): Hide the visibility of the label. The label remains visible for screen readers. Defauls to `false`.

## Styling

The `TextInput` component can be styled using CSS classes or styled-components. Customize it to match the design requirements of your project.
