# Frame Component

The `Image` component is used to display images in various aspect ratios. Below are the guidelines for using the `Image` component effectively.

## Aspect Ratios

### Portrait
- **Aspect Ratio**: 3:4
- **Usage**: Suitable for displaying images that are taller than they are wide.

### Landscape
- **Aspect Ratio**: 4:3
- **Usage**: Ideal for images that are wider than they are tall.

### Square
- **Aspect Ratio**: 1:1
- **Usage**: Best for images that need to be displayed with equal width and height.

## Example Usage

```jsx
import { Frame } from 'octagon-design-system';

const Example = () => (
    <div>
        <Frame src="portrait.jpg" alt="Portrait Image" aspectRatio="3:4" />
        <Frame src="landscape.jpg" alt="Landscape Image" aspectRatio="4:3" />
        <Frame src="square.jpg" alt="Square Image" aspectRatio="1:1" />
    </div>
);
```
Ensure that the `src` attribute points to the correct image path and the `alt` attribute provides a meaningful description of the image.

## Props

- `src` (string): The source URL of the image.
- `alt` (string): The alternative text for the image.
- `aspectRatio` (string): The aspect ratio of the image. Acceptable values are `3:4`, `4:3`, and `1:1`.

By following these guidelines, you can ensure that images are displayed correctly and consistently across your application.