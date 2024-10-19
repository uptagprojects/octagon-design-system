# Tag Component

The `Tag` component is used to display small pieces of information, such as labels or categories.

## Usage

```jsx
import { Tag } from 'octagon-design-system';

function App() {
    return (
        <div>
            <Tag>Example Tag</Tag>
        </div>
    );
}

export default App;
```

## Props

| Prop      | Type   | Description                      |
|-----------|--------|----------------------------------|
| `children`| string | The content to be displayed inside the tag. |

## Example

```jsx
<Tag>New</Tag>
<Tag>Sale</Tag>
<Tag>Featured</Tag>
```

## Customization

You can customize the `Tag` component using CSS or styled-components to fit your design needs.
