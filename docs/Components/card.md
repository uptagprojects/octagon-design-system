# Cards

Cards are versatile containers for displaying content and actions on a single topic.

## Usage

### Props

- `children`* (ReactNode): The content of the card.
- `size` ("small", "medium", "large"): Changes content size. Defaults to `small`.
- `image` (string): URL of the image.
- `alt` (string): Alternative text of the image.
- `aspectRatio` ("square", "portrait", "landscape"): Image aspect ratio. For more information refer to our [Layout Guidelines](../layout.md).


```jsx
import React from 'react';
import { Card, CardHeader, CardFooter } from 'octagon-ui';

const ExampleCard = () => (
  <Card size="medium" image="https://via.placeholder.com/150" alt="Placeholder Image" aspectRatio="landscape">
    <CardHeader title="Card Title" />
    <p>This is an example of a card component using octagon-ui.</p>
    <CardFooter><p>Card Footer</CardFooter>
  </Card>
);

export default ExampleCard;
```

## Best Practices

- Use cards to group related content
- Maintain consistent padding and spacing within cards
- Limit the amount of content in a single card
- Use clear visual hierarchy within the card

Cards are excellent for creating modular, reusable content blocks in your interfaces.