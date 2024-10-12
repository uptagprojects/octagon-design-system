# TextAreaInput Component

The `TextAreaInput` component is used to create multi-line text input fields. It is ideal for collecting longer pieces of text from users, such as comments, descriptions, or messages.

## Usage

### Basic Example

```jsx
import { TextAreaInput } from 'octagon-design-system';

function App() {
    return (
        <TextAreaInput
            label="Description"
            placeholder="Enter your description here..."
        />
    );
}
```

### Props

- `label` (string): The label for the text area.
- `placeholder` (string): The placeholder text displayed inside the text area.
- `value` (string): The current value of the text area.
- `onChange` (function): Callback function to handle changes to the text area value.
- `disabled` (boolean): If true, the text area will be disabled.
- `rows` (number): The number of visible text lines for the control.

### Example with All Props

```jsx
import { TextAreaInput } from 'octagon-design-system';

function App() {
    const [value, setValue] = useState('');

    const handleChange = (event) => {
        setValue(event.target.value);
    };

    return (
        <TextAreaInput
            label="Comments"
            placeholder="Enter your comments here..."
            value={value}
            onChange={handleChange}
            disabled={false}
            rows={5}
        />
    );
}
```

## Best Practices

- Use clear and concise labels to describe the expected input.
- Provide a placeholder to guide users on what to enter.
- Ensure the text area is appropriately sized for the expected input length.
- Handle the `onChange` event to manage the state of the input.

By following these guidelines, you can effectively use the `TextAreaInput` component to enhance user input experiences in your application.