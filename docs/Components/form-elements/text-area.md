# TextAreaInput Component

The `TextAreaInput` component is used to create multi-line text input fields. It is ideal for collecting longer pieces of text from users, such as comments, descriptions, or messages.

## Usage

```jsx
import { TextArea } from 'octagon-ui';

function App() {
    return (
        <TextArea
            label="Description"
            placeholder="Enter your description here..."
        />
    );
}
```

### Props

The `TextArea` component accepts any of the `<textarea />` props, plus the following:

- `label`* (string): The label for the text area.
- `placeholder` (string): The placeholder text displayed inside the text area.
- `size` ("small", "medium", "large"): The size of the text area. Defaults to `medium`.
- `hideLabel` (boolean): Hide the visibility of the label. The label remains visible for screen readers. Defauls to `false`.


## Best Practices

- Use clear and concise labels to describe the expected input.
- Provide a placeholder to guide users on what to enter.
- Ensure the text area is appropriately sized for the expected input length.
- Handle the `onChange` event to manage the state of the input.

By following these guidelines, you can effectively use the `TextAreaInput` component to enhance user input experiences in your application.