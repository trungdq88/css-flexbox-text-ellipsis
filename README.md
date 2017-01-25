# CSS Flexbox Text Ellipsis

Use: `min-width: 0`, `text-overflow: ellipsis` and `white-space: nowrap`.

## HTML
```html
  <div class="target">
    <div class="target-title">
      Text here is very very long that it might
      get truncate if this box get resized too small
    </div>
    <div class="target-button">
      Button
    </div>
  </div>
```

## CSS
```css
  .target {
    display: flex;
    width: 100%;
    justify-content: space-between;
    align-items: center;
  }

  .target-title {
    overflow: hidden;
    padding: 5px;
    min-width: 0;
    text-overflow: ellipsis;
    white-space: nowrap;
  }

  .target-button {
    padding: 5px 10px;
    background: #2196F3;
    color: white;
  }
```
