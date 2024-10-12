# Tabs Component

The Tabs component is used to organize content into separate views, allowing users to navigate between them easily. Below are the guidelines for using the Tabs component effectively.

## Usage

### Basic Example

```html
<div class="tabs">
    <ul class="tab-list">
        <li class="tab active" data-tab="tab-1">Tab 1</li>
        <li class="tab" data-tab="tab-2">Tab 2</li>
        <li class="tab" data-tab="tab-3">Tab 3</li>
    </ul>
    <div class="tab-content active" id="tab-1">
        Content for Tab 1
    </div>
    <div class="tab-content" id="tab-2">
        Content for Tab 2
    </div>
    <div class="tab-content" id="tab-3">
        Content for Tab 3
    </div>
</div>
```

### JavaScript Initialization

To make the tabs functional, you need to add JavaScript to handle the tab switching.

```javascript
document.querySelectorAll('.tab').forEach(tab => {
    tab.addEventListener('click', () => {
        document.querySelectorAll('.tab, .tab-content').forEach(item => {
            item.classList.remove('active');
        });
        tab.classList.add('active');
        document.getElementById(tab.getAttribute('data-tab')).classList.add('active');
    });
});
```

## Best Practices

- **Accessibility**: Ensure that the tabs are accessible by using appropriate ARIA roles and keyboard navigation.
- **Responsive Design**: Make sure the tabs are responsive and work well on different screen sizes.
- **Consistent Styling**: Maintain consistent styling across all tabs for a uniform look and feel.

## Accessibility

To enhance accessibility, use the following ARIA attributes:

```html
<ul class="tab-list" role="tablist">
    <li class="tab active" role="tab" aria-selected="true" aria-controls="tab-1" id="tab-1-tab">Tab 1</li>
    <li class="tab" role="tab" aria-selected="false" aria-controls="tab-2" id="tab-2-tab">Tab 2</li>
    <li class="tab" role="tab" aria-selected="false" aria-controls="tab-3" id="tab-3-tab">Tab 3</li>
</ul>
<div class="tab-content active" role="tabpanel" id="tab-1" aria-labelledby="tab-1-tab">
    Content for Tab 1
</div>
<div class="tab-content" role="tabpanel" id="tab-2" aria-labelledby="tab-2-tab">
    Content for Tab 2
</div>
<div class="tab-content" role="tabpanel" id="tab-3" aria-labelledby="tab-3-tab">
    Content for Tab 3
</div>
```

By following these guidelines, you can ensure that the Tabs component is used effectively and provides a good user experience.