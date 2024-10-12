---
sidebar_position: 5
---

# Design Tokens

Design tokens are the core pieces of a design system, representing the values and styles used throughout the project. They ensure consistency and scalability in design. In the Octagon Design System, we use three types of tokens: constant, semantic, and contextual.

## Types of Tokens

### Constant Tokens
Constant tokens are the fundamental values that do not change. They include colors, typography scales, spacing units, etc.

Example:
```json
{
    "color-primary": "#3498db",
    "font-size-base": "16px",
    "spacing-small": "8px"
}
```

### Semantic Tokens
Semantic tokens map constant tokens to specific design elements, providing meaningful names that describe their purpose.

Example:
```json
{
    "button-background": "{color-primary}",
    "text-body": "{font-size-base}",
    "margin-small": "{spacing-small}"
}
```

### Contextual Tokens
Contextual tokens adapt semantic tokens to different contexts or themes, allowing for variations in design based on usage or environment.

Example:
```json
{
    "button-background-dark": "#2980b9",
    "text-body-large": "18px",
    "margin-small-mobile": "4px"
}
```

By using these tokens, we maintain a consistent and adaptable design system that can easily scale and evolve.