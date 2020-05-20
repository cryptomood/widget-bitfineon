## Configuration
To configure the widget, either pass an HTML attribute, or a query string to the component.

## Configuration options
- **asset** - The asset to track. Defaults to `BTC`.
- **theme** - The theme to use. Options are `light` & `dark`. Defaults to `light`.
- **showToggle** - Whether the hiding toggle should be displayed. Options are `true` & `false`. Defaults to `false`.
- **animate** - Whether the widget hiding should be animated. Options are `true` & `false`. Defaults to `true`.
- **newsOnly** - Whether the widget should display an alternate news-only view with content preview & image. Options are "true" & "false". Defaults to `false`.

## Handling toggled widget state
The widget exposes two methods to `get` and `set` the `toggled` state externally.

- `getIsWidgetOpen: () => boolean` - Returns a boolean value corresponding to the current toggled state.
- `setIsWidgetOpen: (boolean) => void` - Accepts a variable defining whether the widget should close or not.

Example:
```js
// Default state is open
document.getElementById("pepe").setIsWidgetOpen(false)
> undefined
document.getElementById("pepe").getIsWidgetOpen()
> false
document.getElementById("pepe").setIsWidgetOpen(true)
> undefined
document.getElementById("pepe").getIsWidgetOpen()
> true
```
