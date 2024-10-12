# Checkbox Component

The Checkbox component is used to allow users to select one or more options from a set. Below is a guide on how to use the Checkbox component in your project.

## Usage

### Basic Example

```html
<label>
    <input type="checkbox" name="example" value="1">
    Option 1
</label>
<label>
    <input type="checkbox" name="example" value="2">
    Option 2
</label>
```

### Props

- `name`: The name attribute for the checkbox input.
- `value`: The value attribute for the checkbox input.
- `checked`: Determines whether the checkbox is checked by default.
- `disabled`: Disables the checkbox if set to true.

### Example with Props

```html
<label>
    <input type="checkbox" name="example" value="1" checked>
    Option 1 (Checked by default)
</label>
<label>
    <input type="checkbox" name="example" value="2" disabled>
    Option 2 (Disabled)
</label>
```

### Accessibility

Ensure that each checkbox has an associated `<label>` to improve accessibility. The `for` attribute of the `<label>` should match the `id` of the checkbox input.

```html
<label for="option1">Option 1</label>
<input type="checkbox" id="option1" name="example" value="1">
```

## Conclusion

The Checkbox component is a versatile form element that can be used in various scenarios to allow users to make multiple selections. Ensure to use proper labels and attributes to enhance accessibility and usability.