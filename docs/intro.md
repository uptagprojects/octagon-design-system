---
sidebar_position: 1
---

# Getting Started

Octagon is a comprehensive design system that provides a unified language for creating consistent, beautiful, and user-friendly interfaces. It is built on the principles of flexibility, accessibility, and scalability.

## Why Octagon?

- **Consistency**: Ensure a cohesive look and feel across all your products and platforms.
- **Simplicity**: Keep designs clean and intuitive for users.
- **Efficiency**: Speed up your design and development process with pre-built components and patterns.
- **Flexibility**: Easily customize and extend the system to meet your specific needs.
- **Accessibility**: Built with accessibility in mind to create inclusive user experiences.
- **Performance**: Optimize for speed and efficiency in both design and code.

These principles guide all aspects of the Octagon Design System, from color choices to component design and implementation.

## Getting Started

### Installation

To start using Octagon in your project, you need to install the package via npm. Follow these steps:

1. Open your terminal.
2. Navigate to your project directory.
3. Run the following command to install Octagon:

  ```sh
  npm install octagon-ui
  ```

Import the `index.css` file into your main component to load all the styles:

```
// App.js
import "octagon-ui/dist/index.css";

// ...
```

After the installation is complete, you can start importing and using Octagon components in your project.

```javascript
import { Button } from 'octagon-ui';

function App() {
  return <Button label="Click me" />;
}
```

For more details on how to use the components, refer to the [Components](./Components/avatar.md) section of the documentation.

You can also explore our documentation:

1. [Layout Guidelines](./layout.md)
2. [Color System](./colors.md)
3. [Typography](./typography.md)
4. [Components](./Components/avatar.md)
5. [Patterns](./Patterns/data-display.md)


Let's create beautiful and functional interfaces together with Octagon!
