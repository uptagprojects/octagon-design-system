# Switch Component

The Switch component is used to toggle between two states, such as on/off or true/false. It is commonly used in forms and settings.

## Usage

### Basic Example

```jsx
import { Switch } from 'octagon-design-system';

function Example() {
    const [isOn, setIsOn] = useState(false);

    return (
        <Switch
            checked={isOn}
            onChange={() => setIsOn(!isOn)}
        />
    );
}
```

### Props

- `checked` (boolean): Determines whether the switch is in the "on" state.
- `onChange` (function): Callback function that is called when the switch is toggled.

### Accessibility

Ensure that the Switch component is accessible by providing appropriate labels and using ARIA attributes if necessary.

```jsx
<Switch
    checked={isOn}
    onChange={() => setIsOn(!isOn)}
    aria-label="Toggle setting"
/>
```

### Best Practices

- Use clear and descriptive labels to indicate what the switch controls.
- Avoid using switches for actions that require immediate feedback or confirmation.

## Examples

### Controlled Component

```jsx
function ControlledSwitch() {
    const [isChecked, setIsChecked] = useState(false);

    const handleChange = (event) => {
        setIsChecked(event.target.checked);
    };

    return (
        <Switch
            checked={isChecked}
            onChange={handleChange}
        />
    );
}
```

### Uncontrolled Component

```jsx
function UncontrolledSwitch() {
    return (
        <Switch defaultChecked />
    );
}
```

By following these guidelines, you can effectively use the Switch component in your projects.