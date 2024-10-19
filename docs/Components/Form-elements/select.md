# Select Component

The `Select` component is used to create a dropdown list that allows users to choose one option from a predefined set of options.

## Usage

### Basic Example

```jsx
import { Select } from 'octagon-design-system';

const options = [
    { value: 'option1', label: 'Option 1' },
    { value: 'option2', label: 'Option 2' },
    { value: 'option3', label: 'Option 3' },
];

function App() {
    return (
        <Select options={options} />
    );
}
```

### Props

- `options` (array): An array of objects representing the options. Each object should have a `value` and a `label` property.
- `onChange` (function): A callback function that is called when the selected option changes.
- `value` (string): The currently selected value.

### Example with onChange

```jsx
import { Select } from 'octagon-design-system';
import { useState } from 'react';

const options = [
    { value: 'option1', label: 'Option 1' },
    { value: 'option2', label: 'Option 2' },
    { value: 'option3', label: 'Option 3' },
];

function App() {
    const [selectedOption, setSelectedOption] = useState(options[0].value);

    const handleChange = (event) => {
        setSelectedOption(event.target.value);
    };

    return (
        <Select options={options} value={selectedOption} onChange={handleChange} />
    );
}
```

### Custom Styling

You can customize the appearance of the `Select` component using CSS or styled-components.

```jsx
import styled from 'styled-components';
import { Select } from 'octagon-design-system';

const CustomSelect = styled(Select)`
    border: 2px solid #007bff;
    border-radius: 4px;
    padding: 8px;
`;

const options = [
    { value: 'option1', label: 'Option 1' },
    { value: 'option2', label: 'Option 2' },
    { value: 'option3', label: 'Option 3' },
];

function App() {
    return (
        <CustomSelect options={options} />
    );
}
```

## Accessibility

Ensure that the `Select` component is accessible by providing appropriate `aria` attributes and labels.

```jsx
<Select
    options={options}
    aria-label="Select an option"
    aria-required="true"
/>
```

## Conclusion

The `Select` component is a versatile and essential part of any form. By following the examples and guidelines provided, you can effectively integrate it into your application.