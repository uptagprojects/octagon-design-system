# Container

The `<Container>` component is used to wrap content and center it within its parent.

## Usage

Simply import it and set the `center` prop as needed.


## Props

- `center` (boolean): When set to `true`, the content inside the `<Container>` will be centered. Defaults to `false`.

## Example

```jsx
import React from 'react';
import { Container } from 'octagon-ui';

const Example = () => (
    <Container center={true}>
        <p>This content is centered.</p>
    </Container>
);

export default Example;
```
