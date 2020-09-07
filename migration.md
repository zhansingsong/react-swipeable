# React Swipeable v6 changes and migration

## New Features

- addition of `onTap` event handler prop which executes the callback after a tap

## Major Changes

- removal of `<Swipeable>` component
  - _TODO_ add example for creating one and migrating
- update calculation of `deltaX` and `deltaY` from `initial - current` to `current - initial`
  - Example: `const deltaX = state.xy[0] - x;` is now `const deltaX = x - state.xy[0];`
- add new `vxvy` vector which contains velocity per each dimension

## Migrate Swipeable v5 to v6