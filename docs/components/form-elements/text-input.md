# TextInput Component

The `TextInput` component is a versatile input field used for collecting user input in the form of text. It is commonly used in forms and can be customized to fit various use cases.

## Usage

To use the `TextInput` component, import it into your project and include it in your JSX:

```jsx
import { TextInput } from 'octagon-design-system';

function MyForm() {
    return (
        <form>
            <label htmlFor="username">Username:</label>
            <TextInput id="username" name="username" placeholder="Enter your username" />
        </form>
    );
}
```

## Props

The `TextInput` component accepts the following props:

- **id** (string): A unique identifier for the input field.
- **name** (string): The name attribute for the input field.
- **placeholder** (string): A placeholder text that appears when the input is empty.
- **value** (string): The current value of the input field.
- **onChange** (function): A callback function that is called when the input value changes.
- **disabled** (boolean): If true, the input field will be disabled.

## Example

```jsx
import React, { useState } from 'react';
import { TextInput } from 'octagon-design-system';

function Example() {
    const [value, setValue] = useState('');

    const handleChange = (event) => {
        setValue(event.target.value);
    };

    return (
        <div>
            <label htmlFor="example">Example Input:</label>
            <TextInput
                id="example"
                name="example"
                placeholder="Type something..."
                value={value}
                onChange={handleChange}
            />
        </div>
    );
}
```

## Accessibility

Ensure that each `TextInput` has an associated label for better accessibility. Use the `id` and `htmlFor` attributes to link the input field with its label.

## Styling

The `TextInput` component can be styled using CSS or styled-components. Customize it to match the design requirements of your project.
