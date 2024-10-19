# Date Picker Component

The Date Picker component allows users to select a date from a calendar or enter it manually. This component is part of the Octagon Design System.

## Usage

### Basic Example

```html
<DatePicker />
```

### Props

- `value`: The selected date.
- `onChange`: Callback function when the date is changed.
- `minDate`: The minimum selectable date.
- `maxDate`: The maximum selectable date.

### Example with Props

```html
<DatePicker 
    value={selectedDate} 
    onChange={handleDateChange} 
    minDate="2023-01-01" 
    maxDate="2023-12-31" 
/>
```

### Accessibility

Ensure that the Date Picker is accessible by providing appropriate labels and descriptions.

### Customization

You can customize the appearance of the Date Picker using CSS or by overriding default styles.

For more details, refer to the [Octagon Design System documentation](https://example.com/docs).
