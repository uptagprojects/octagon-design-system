---
sidebar_position: 2
---

# Layout

## Grid System

Octagon uses a flexible grid system to create consistent layouts across different screen sizes.

### Usage

```jsx
<Container center={true}>
  Welcome to PNFi
</Container>
```

This grid system provides a solid foundation for creating responsive and consistent layouts in your projects.

## Responsive Design

Octagon emphasizes responsive design to ensure optimal user experiences across various devices and screen sizes.

### Breakpoints

- XS: < 640px Average Mobile size
- SM: >=640px Portrait Tablet
- MD: >=768px Landscape Tablet, or a Small Desktop
- LG: >=1024px Standard Desktop size
- XL: >=1280px Standard to large Desktop size

### Best Practices

1. Mobile-first approach
2. Fluid typography
3. Flexible images and media
4. Considerate use of white space
5. Progressive enhancement

By following these responsive design principles, you can create interfaces that adapt seamlessly to different screen sizes and devices.

## Fixed Width Containers

Octagon also provides fixed-width containers for scenarios where a consistent width is required. These containers are particularly useful for layouts with many horizontal components or large elements like tables.

### Available Content Widths

- **900px**: Standard fixed width for most layouts.
- **1024px**: Use this width when dealing with many horizontal components or large elements.
- Full width: Used on animations, full-sized parallax or slides, charts, and sections where the interaction benefits from more screen real-estate.

### Usage

The fixed container width is included in all the direct children of body: `<main>`, `<nav>` and `<footer>`. This is the grid spec:


| header | header  | header |
| ------ | ------- | ------ |
| .      | content | .      |
| footer | footer  | footer |

You can access and use it being a direct children of the body:

```css

body > .my_component {
  grid-area: footer;
  display: grid;
  grid-template-columns: subgrid;
}

```

These fixed-width containers help maintain a consistent layout, especially when dealing with complex or large horizontal elements.

## Fluid Container

In addition to fixed-width containers, Octagon also supports fluid containers that span the entire width of the viewport. This is particularly useful for creating layouts that need to adapt to various screen sizes without fixed constraints. The fluid container width is included in all the children nodes of `<main>`.

We included the body as a container, in order to use CSS `@container` queries. You can access it with `oct-body`:

```css
.my_component {
  width: 320px;

  @container oct-body (min-width: 768px) {
    width: 480px;
  }
}
```


### Aspect Ratios

#### Portrait
- **Aspect Ratio**: 3:4
- **Usage**: Suitable for displaying images that are taller than they are wide.

#### Landscape
- **Aspect Ratio**: 16:9
- **Usage**: Ideal for videos, full-screen components, and images that are wider than they are tall.

#### Square
- **Aspect Ratio**: 1:1
- **Usage**: Best for images that need to be displayed with equal width and height. Ideal for embeds.