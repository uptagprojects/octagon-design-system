# Dialog Component

The `Dialog` component is used to display important information or prompt the user for a decision. It appears as a modal window, blocking interaction with the rest of the application until it is dismissed.

## Usage

### Basic Example

```jsx
import { Dialog } from 'octagon-design-system';

function App() {
    const [isOpen, setIsOpen] = useState(false);

    return (
        <>
            <button onClick={() => setIsOpen(true)}>Open Dialog</button>
            <Dialog isOpen={isOpen} onClose={() => setIsOpen(false)}>
                <Dialog.Header>Dialog Title</Dialog.Header>
                <Dialog.Body>
                    <p>This is the content of the dialog.</p>
                </Dialog.Body>
                <Dialog.Footer>
                    <button onClick={() => setIsOpen(false)}>Close</button>
                </Dialog.Footer>
            </Dialog>
        </>
    );
}
```

### Props

- `isOpen` (boolean): Controls the visibility of the dialog.
- `onClose` (function): Callback function triggered when the dialog is requested to be closed.

### Subcomponents

- `Dialog.Header`: Defines the header section of the dialog.
- `Dialog.Body`: Defines the main content area of the dialog.
- `Dialog.Footer`: Defines the footer section of the dialog, typically containing action buttons.

## Best Practices

- Ensure the dialog is accessible by providing appropriate ARIA roles and labels.
- Keep the content concise and relevant to the user's current task.
- Avoid nesting dialogs to prevent overwhelming the user.

## Accessibility

- Use `aria-labelledby` and `aria-describedby` to associate the dialog with its title and content.
- Ensure focus management by trapping focus within the dialog and returning focus to the triggering element when closed.

By following these guidelines, you can effectively use the `Dialog` component to enhance user interaction in your application.