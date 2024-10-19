# Avatar Component
The Avatar component in the Octagon Design System is a unique and visually distinct element. Unlike conventional circular avatars, our Avatar component features an outlined octagon shape, making it stand out in any user interface.

## Features

- **Octagon Shape**: The primary feature of our Avatar component is its outlined octagon shape, providing a modern and unique look.
- **Customizable**: Easily customize the size, border color, and background color to fit your design needs.
- **Responsive**: The Avatar component is fully responsive and looks great on all devices.

## Usage

### Props

- `src`* (string): The URL of the image.
- `alt`* (string): Alternative text for accesibility.
- `size` (number): Avatar size in pixels. Defaults to 50px.


## Example

```jsx
import React from 'react';
import { Avatar } from 'octagon-ui';

const UserProfile = () => {
    return (
        <div>
            <h2>User Profile</h2>
            <Avatar src="/user.jpg" alt="Jane Doe profile picture" size={120} />
        </div>
    );
};

export default UserProfile;
```
