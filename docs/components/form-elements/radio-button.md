# Radio Button Component

The Radio Button component is used to allow users to select one option from a set of mutually exclusive options. Below is a guide on how to properly use the Radio Button component in your project.

## Usage

### Basic Example

```html
<form>
    <label>
        <input type="radio" name="option" value="1">
        Option 1
    </label>
    <label>
        <input type="radio" name="option" value="2">
        Option 2
    </label>
</form>
```

### Grouping Radio Buttons

Ensure that all radio buttons in a group share the same `name` attribute. This groups them together, allowing only one to be selected at a time.

```html
<form>
    <label>
        <input type="radio" name="group1" value="1">
        Group 1 - Option 1
    </label>
    <label>
        <input type="radio" name="group1" value="2">
        Group 1 - Option 2
    </label>
    <label>
        <input type="radio" name="group1" value="3">
        Group 1 - Option 3
    </label>
</form>
```

### Disabled State

To disable a radio button, add the `disabled` attribute.

```html
<form>
    <label>
        <input type="radio" name="option" value="1" disabled>
        Disabled Option
    </label>
</form>
```

### Pre-selected Option

To pre-select a radio button, add the `checked` attribute.

```html
<form>
    <label>
        <input type="radio" name="option" value="1" checked>
        Pre-selected Option
    </label>
</form>
```

## Accessibility

- Ensure each radio button has an associated `<label>` for better accessibility.
- Use `aria-checked` to indicate the current state of the radio button if you are using custom radio buttons.

```html
<label>
    <input type="radio" name="option" value="1" aria-checked="false">
    Option 1
</label>
<label>
    <input type="radio" name="option" value="2" aria-checked="true">
    Option 2
</label>
```

## Conclusion

The Radio Button component is a simple yet powerful tool for creating forms with mutually exclusive options. By following the guidelines above, you can ensure that your radio buttons are both functional and accessible.
