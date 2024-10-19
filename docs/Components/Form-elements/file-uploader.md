# FileUploader Component

The `FileUploader` component is used to upload files in a form. Below are the guidelines and examples for its proper usage.

## Usage

### Basic Example

```jsx
import { FileUploader } from 'octagon-design-system';

function App() {
    return (
        <FileUploader
            label="Upload your file"
            onChange={(files) => console.log(files)}
        />
    );
}
```

### Props

- `label` (string): The label for the file uploader.
- `onChange` (function): Callback function that is called when files are selected.

### Advanced Example

```jsx
import { FileUploader } from 'octagon-design-system';

function App() {
    const handleFileChange = (files) => {
        // Handle file upload logic here
        console.log('Selected files:', files);
    };

    return (
        <FileUploader
            label="Upload your documents"
            multiple={true}
            accept=".pdf,.docx"
            onChange={handleFileChange}
        />
    );
}
```

### Additional Props

- `multiple` (boolean): Allows multiple file selection.
- `accept` (string): Specifies the types of files that the server accepts (e.g., `.pdf,.docx`).

## Best Practices

- Always provide a clear and concise label.
- Use the `accept` prop to restrict file types for better validation.
- Handle file uploads asynchronously to improve user experience.

## Accessibility

Ensure the `FileUploader` component is accessible by providing appropriate labels and handling focus states.
