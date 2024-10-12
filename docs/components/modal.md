# Modal Component

The Modal component is used to display content in a layer above the app. It is often used for dialogs, alerts, or forms that require user interaction.

## Usage

### Basic Example

```jsx
import { Modal } from 'octagon-design-system';

function App() {
    const [isOpen, setIsOpen] = useState(false);

    return (
        <>
            <button onClick={() => setIsOpen(true)}>Open Modal</button>
            <Modal isOpen={isOpen} onClose={() => setIsOpen(false)}>
                <h2>Modal Title</h2>
                <p>Modal content goes here.</p>
                <button onClick={() => setIsOpen(false)}>Close</button>
            </Modal>
        </>
    );
}
```

### Props

- `isOpen` (boolean): Controls the visibility of the modal.
- `onClose` (function): Callback function triggered when the modal is requested to be closed.

### Accessibility

Ensure that the modal is accessible by:
- Setting the `aria-labelledby` attribute to the ID of the modal title.
- Setting the `aria-describedby` attribute to the ID of the modal content.

### Best Practices

- Keep the modal content concise and focused.
- Avoid nesting modals.
- Ensure the modal can be closed using the `Esc` key and a close button.

## Conclusion

The Modal component is a powerful tool for creating interactive dialogs. By following the usage guidelines and best practices, you can create accessible and user-friendly modals in your application.