# Avatar Component
The Avatar component in the Octagon Design System is a unique and visually distinct element. Unlike conventional circular avatars, our Avatar component features an outlined octagon shape, making it stand out in any user interface.

## Features

- **Octagon Shape**: The primary feature of our Avatar component is its outlined octagon shape, providing a modern and unique look.
- **Customizable**: Easily customize the size, border color, and background color to fit your design needs.
- **Responsive**: The Avatar component is fully responsive and looks great on all devices.

## Usage

To use the Avatar component, simply include it in your project and customize it as needed:


```jsx
import React from 'react';
import { Avatar } from 'octagon-ui';

const UserProfile = () => {
    return (
        <div>
            <h2>User Profile</h2>
            <Avatar src="user.jpg" alt="Jane Doe" size="large" />
        </div>
    );
};

export default UserProfile;
```
