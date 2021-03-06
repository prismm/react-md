Navigation drawers have 7 types:

```js
const {
  FULL_HEIGHT,
  CLIPPED,
  FLOATING,
  PERSISTENT,
  PERSISTENT_MINI,
  TEMPORARY,
  TEMPORARY_MINI,
} = NavigationDrawer.DrawerType;
```

The `TEMPORARY` or `TEMPORARY_MINI` *must* be used for mobile devices. The
default media queries will already handle this for you. If the `drawerType`
is set to anything except for `PERSISTENT_MINI`, the mobile version of the
drawer will automatically be `TEMPORARY`. If the `drawerType` is set to
`PERSISTENT_MINI`, then the mobile version will be `TEMPORARY_MINI`.

If you would like a consistent `drawerType` between all devices, you can
always set the `drawerType` to `TEMPORARY` or `TEMPORARY_MINI`.

### NavigationDrawer vs Drawer/Toolbar
The `NavigationDrawer` component is just a simple way to combine a main fixed `Toolbar` and a `Drawer`
component on the page. It will handle any of the positioning and offsets required for you. It will definitely
be less flexible than the `Drawer/Toolbar` manual combo yourself.
