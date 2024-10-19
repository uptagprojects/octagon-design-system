# Frame Component

The `Image` component is used to display images in various aspect ratios. Below are the guidelines for using the `Image` component effectively.



## Example Usage

```jsx
import React from "react";
import { Frame } from "octagon-ui";

const Example = () => (
    <div>
        <Frame src="portrait.jpg" alt="Portrait Image" aspectRatio="portrait" />
        <Frame src="landscape.jpg" alt="Landscape Image" aspectRatio="landscape" />
        <Frame src="square.jpg" alt="Square Image" aspectRatio="square" />
    </div>
);
```
Ensure that the `src` attribute points to the correct image path and the `alt` attribute provides a meaningful description of the image.

## Props

- `src`* (string): The source URL of the image.
- `alt`* (string): The alternative text for the image.
- `aspectRatio` ("square", "landscape", "portrait"): The aspect ratio of the image. For more information refer to our [Layout Guidelines](../layout.md).

By following these guidelines, you can ensure that images are displayed correctly and consistently across your application.