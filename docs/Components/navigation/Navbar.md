# Header Component
The `Navbar` component is a crucial part of the Octagon Design System. It provides a consistent and customizable navigation bar for your application.

## Usage

To use the `Navbar` component, follow these steps:

1. **Import the Component:**
  ```javascript
  import { Navbar } from 'octagon-ui';
  ```

2. **Basic Example:**
  The `Navbar` component is a crucial part of the Octagon Design System. It provides a consistent and customizable navigation bar for your application.

  ## Usage

  To use the `Navbar` component, follow these steps:

  1. **Import the Component:**
    ```javascript
    import { Navbar, NavItem } from 'octagon-ui';
    ```

  2. **Basic Example:**
    ```jsx
    <Navbar>
      <div>My Application</div>
    </Navbar>
    ```

  3. **Props:**
    - `brand` (ReactNode): The brand element to be displayed in the navbar.
    - `children` (ReactNode): The children elements to be displayed in the navbar.
    - `callToAction` (ReactNode): The call-to-action element to be displayed in the navbar.

    ```jsx
    const navigationItems = (
      <ul>
        <NavItem active={true}><a href="/">Home</a></NavItem>
        <NavItem><a href="/about">About</a></NavItem>
        <NavItem><a href="/contact">Contact</a></NavItem>
      </ul>
    );

    <Navbar 
      brand={<img src="/path/to/logo.png" alt="Logo" />} 
      callToAction={<button>Sign Up</button>}
    >
      {navigationItems}
    </Navbar>
    ```

  4. **Styling:**
    The `Navbar` component can be styled using CSS classes or inline styles. It is recommended to use the provided CSS classes for consistency.

    ```jsx
    <Navbar 
      brand={<div>My Application</div>} 
      className="custom-navbar" 
    />
    ```

  ## Best Practices

  - Ensure the `brand` is concise and descriptive.
  - Use a high-resolution logo for better display quality.
  - Keep the navigation items relevant and limited to essential links.

  ## Accessibility

  - Use semantic HTML elements within the `Navbar` component.
  - Ensure the navbar is keyboard navigable.
  - Provide alt text for the logo image.

  By following these guidelines, you can effectively utilize the `Navbar` component in your projects.
