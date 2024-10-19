---
sidebar_position: 3
---

# Spacing

Proper use of spacing is crucial for creating clear visual hierarchies and improving readability. Octagon uses a consistent spacing scale to maintain visual harmony throughout the interface.


## General Rules

1. Use consistent spacing within component groups
2. Increase spacing between distinct sections
3. Align elements to the spacing grid
4. Use white space strategically to guide user focus


## Space Guidelines

### Scale

1. **2px or 4px** - Used for spacing within a component
  - Example: Padding inside a button or input field.
2. **8px** - Used to separate related elements
  - Example: Margin between icons and text within a button.
3. **16px** - Used to separate unrelated elements
  - Example: Space between different buttons in a toolbar.
4. **24px** - Used to separate sub-sections of content
  - Example: Margin between a section title and its content.
5. **32px** - Used to separate sections of content
  - Example: Space between different sections on a webpage.
6. **40px** - Used for larger separations within sections
  - Example: Padding around a card component.
7. **48px** - Used for major section separations
  - Example: Space between the main content and a sidebar.
8. **56px** - Used for separating large content blocks
  - Example: Margin between large images or videos.
9. **64px** - Used for separating very large content blocks
  - Example: Space between major sections on a landing page.
10. **72px** - Used for separating distinct content areas
   - Example: Margin between the header and the main content.
11. **80px** - Used for separating major content areas
   - Example: Space between the main content and the footer.
12. **96px** - Used for the largest separations in layouts
   - Example: Padding around a full-page modal or overlay.

By adhering to these scales, you can ensure a consistent and harmonious layout throughout your design.

### Usage

You can access all of the sizes and scales with the variables `--size-{number}` and `--scale-{number}`:

```css
.my_component {
  padding: var(--scale-2);
  font-size: var(--size-4);
}
```