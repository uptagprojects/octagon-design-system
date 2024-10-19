# Buttons

Buttons are essential interactive elements in user interfaces. Octagon provides a variety of button styles to suit different needs.

## Button Variants

This is the hierarchy of the buttons.

1. Primary
2. Secondary
3. Tertiary


### Props

- `label`* (string): Button text.
- `variant` ("primary", "secondary", "tertiary"): Button variants. Defaults to `secondary`.
- `size` ("small", "medium", "large"): Button width and text. Defaults to `medium`.

## Usage

```jsx
import React from 'react';
import { Button } from 'octagon-ui';

const App = () => (
    <div>
        <Button variant="primary" label="reserve a seat" />
    </div>
);

export default App;
```

## Best Practices

- Use primary buttons for main actions
- A primary button is used as a Call to Action
- Limit the use of multiple primary buttons on a single page
- Limit the use of a primary button to only one per button group
- Ensure sufficient contrast and touch target size for accessibility
- Icon buttons shall be accompanied with the label

By following these guidelines, you'll create clear and effective call-to-actions in your user interfaces.