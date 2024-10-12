# Header Component

The `Header` component is a crucial part of the Octagon Design System. It provides a consistent and customizable header for your application.

## Usage

To use the `Header` component, follow these steps:

1. **Import the Component:**
    ```javascript
    import { Header } from 'octagon-design-system';
    ```

2. **Basic Example:**
    ```jsx
    <Header title="My Application" />
    ```

3. **Props:**
    - `title` (string): The title to be displayed in the header.
    - `logo` (string): URL of the logo image.
    - `navigation` (array): Array of navigation items.

    ```jsx
    const navigationItems = [
      { name: 'Home', link: '/' },
      { name: 'About', link: '/about' },
      { name: 'Contact', link: '/contact' }
    ];

    <Header 
      title="My Application" 
      logo="/path/to/logo.png" 
      navigation={navigationItems} 
    />
    ```

4. **Styling:**
    The `Header` component can be styled using CSS classes or inline styles. It is recommended to use the provided CSS classes for consistency.

    ```jsx
    <Header 
      title="My Application" 
      className="custom-header" 
    />
    ```

## Best Practices

- Ensure the `title` is concise and descriptive.
- Use a high-resolution logo for better display quality.
- Keep the navigation items relevant and limited to essential links.

## Accessibility

- Use semantic HTML elements within the `Header` component.
- Ensure the header is keyboard navigable.
- Provide alt text for the logo image.

By following these guidelines, you can effectively utilize the `Header` component in your projects.