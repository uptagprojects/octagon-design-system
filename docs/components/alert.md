# Alert Component

The `Alert` component is used to display important messages to the user. It can be used to show success, error, warning, or informational messages.

## Usage

### Importing the Alert Component

First, import the `Alert` component into your file:

```javascript
import { Alert } from 'octagon-design-system';
```

### Basic Example

Here is a basic example of how to use the `Alert` component:

```javascript
<Alert type="success" message="This is a success alert!" />
```

### Alert Types

The `Alert` component supports the following types:

- `success`: Indicates a successful or positive action.
- `error`: Indicates an error or a negative action.
- `warning`: Indicates a warning that might need attention.
- `info`: Indicates informational messages.

### Props

The `Alert` component accepts the following props:

- `type` (string): The type of alert to display. Can be `success`, `error`, `warning`, or `info`.
- `message` (string): The message to display inside the alert.
- `dismissible` (boolean): If true, the alert can be dismissed by the user. Default is `false`.

### Dismissible Alert

To make an alert dismissible, set the `dismissible` prop to `true`:

```javascript
<Alert type="warning" message="This is a warning alert!" dismissible={true} />
```

### Custom Styling

You can apply custom styles to the `Alert` component by using the `className` prop:

```javascript
<Alert type="info" message="This is an informational alert!" className="custom-alert" />
```

## Conclusion

The `Alert` component is a versatile and essential part of the `octagon-design-system`, providing a simple way to communicate important messages to users. By leveraging its various types and properties, you can ensure that your application's alerts are both effective and user-friendly.