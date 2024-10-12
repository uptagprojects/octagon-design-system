# Skeleton Loaders

Skeleton loaders are used to improve the user experience by providing a visual placeholder while content is being loaded. They give users a sense of progress and reduce the perceived waiting time.

## When to Use Skeleton Loaders

- **Data Fetching**: Use skeleton loaders when fetching data from an API or database.
- **Image Loading**: Display skeleton loaders while images are being downloaded.
- **Component Rendering**: Apply skeleton loaders when complex components are being rendered.

## Best Practices

1. **Consistency**: Ensure skeleton loaders match the shape and size of the content they are replacing.
2. **Timing**: Display skeleton loaders immediately when a loading state is detected.
3. **Animation**: Use subtle animations to indicate that the content is loading.
4. **Accessibility**: Make sure skeleton loaders are accessible and provide alternative text for screen readers.

## Example Usage

```html
<div class="skeleton-loader">
    <div class="skeleton-avatar"></div>
    <div class="skeleton-line"></div>
    <div class="skeleton-line short"></div>
</div>
```

## Styling Skeleton Loaders

```css
.skeleton-loader {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.skeleton-avatar {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: #e0e0e0;
}

.skeleton-line {
    height: 20px;
    background: #e0e0e0;
}

.skeleton-line.short {
    width: 60%;
}
```

By following these guidelines, you can effectively use skeleton loaders to enhance the user experience in your application.