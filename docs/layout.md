---
sidebar_position: 2
---

# Layout

## Grid System

Octagon uses a flexible grid system to create consistent layouts across different screen sizes.

### Usage

```jsx
<div className="container">
  <div className="row">
    <div className="col-12">Column 1</div>
    <div className="col-12">Column 2</div>
    <div className="col-12">Column 3</div>
  </div>
</div>
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

To use a fixed-width container, add the appropriate class to your container element:

```jsx
<div className="container-900">
  <div className="row">
    <div className="col-12">Column 1</div>
    <div className="col-12">Column 2</div>
    <div className="col-12">Column 3</div>
  </div>
</div>
```

For the 1024px container, use the `container-1024` class:

```jsx
<div className="container-1024">
  <div className="row">
    <div className="col-12 col-md-6 col-lg-4">Column 1</div>
    <div className="col-12 col-md-6 col-lg-4">Column 2</div>
    <div className="col-12 col-md-6 col-lg-4">Column 3</div>
  </div>
</div>
```

These fixed-width containers help maintain a consistent layout, especially when dealing with complex or large horizontal elements.

## Fluid Container

In addition to fixed-width containers, Octagon also supports fluid containers that span the entire width of the viewport. This is particularly useful for creating layouts that need to adapt to various screen sizes without fixed constraints.

### Usage

To use a fluid container, simply add the `container-fluid` class to your container element:

```jsx
<div className="container-fluid">
  <div className="row">
    <div className="col-12 col-md-6 col-lg-4">Column 1</div>
    <div className="col-12 col-md-6 col-lg-4">Column 2</div>
    <div className="col-12 col-md-6 col-lg-4">Column 3</div>
  </div>
</div>
```

This will ensure that your container spans the full width of the viewport, providing a more flexible and adaptive layout.


