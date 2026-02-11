# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## 2.1.3 (2.1.2 release ignored)
- **`s_sidebar` sub-package improvements**:
  - Enhanced `SideBarController.activateSideBar` with additional customization options:
    - Added `dismissBarrierColor` parameter for custom barrier colors
    - Added `shouldBlurDismissBarrier` parameter for optional blur effect on barrier
    - Added `initState` callback for initialization logic
    - Added `onDismissed` callback to handle sidebar dismissal events

## 2.1.1
- `s_packages` dependency upgraded: **`s_sidebar` sub package upgraded**:
  - `s_sidebar`: Added default left alignment for sidebar activation, allowing the sidebar to stay anchored to the left while minimizing.


## 2.1.0
- ** `s_packages` dependency upgraded: its `s_sidebar`sub-package (along side more packages) was upgraded **:
  - Added `animateFromOffset` to `activateSideBar` to allow animating the sidebar popup from a specific screen position (e.g., button tap location).
  - Added `curve` parameter to customize the animation curve.
  - Added `animationDuration` parameter to control the popup animation speed.
  - Added `useGlobalPosition` parameter to `activateSideBar` and `PopOverlay`, simplifying coordinate handling by automatically converting global tap positions.
  - Fixed an issue where `SSideBar` could error with infinite height constraints when used in an overlay.


## 2.0.0
- package no longer holds the source code for it, but exports/exposes the `s_packages` package instead, which will hold this package's latest source code.
- The only future changes to this package will be made via `s_packages` package dependency upgrades, in order to bring the new fixes or changes to this package
- dependent on `s_packages`: ^1.1.2


## [1.0.3] - 2026-02-05
- Minimise button color/size are now customisable


## [1.0.2] - 2026-02-05
- Minimise button color/shape/size updated


## [1.0.1] - 2026-02-01
- Package Documentation updated


## [1.0.0] - 2026-01-31

### Added
- Initial release of s_sidebar package
- Customizable collapsible sidebar widget for Flutter applications
- Support for minimized and expanded states with smooth animations
- Configurable sidebar items with selected/unselected icons
- Badge support for displaying notifications or counts on menu items
- Tooltip support when sidebar is minimized
- Logo widget support at the top of the sidebar
- Divider option to separate settings item from other items
- Customizable colors for sidebar, icons, text, and background
- Compact mode for reduced spacing between items
- Intelligent layout that adapts to available space
- Automatic height calculation to optimize space usage
- CustomScrollView implementation for efficient scrolling
- Minimize button that stays visible at the bottom
- Responsive design that works with different sidebar heights
- SideBarController for programmatic control
- Support for custom callback when items are tapped
- shouldTapItems parameter to enable/disable specific items
- preSelectedItemIndex to set initial selected item
- Customizable border radius, widths, and item heights
- Customizable horizontal padding, icon-text spacing, and item border radius
- Semantic labels and accessibility support
- Comprehensive test coverage

### Features
- **Adaptive Layout**: Automatically adjusts button expansion based on available space
- **Smooth Animations**: Uses AnimatedContainer and AnimatedAlign for fluid transitions
- **Flexible Styling**: Extensive customization options for colors, sizes, and spacing
- **Accessibility**: Includes Semantics widgets and tooltip support
- **Performance**: Efficient rendering with CustomScrollView and slivers
- **Developer Experience**: Clean API with sensible defaults

[1.0.0]: https://github.com/SoundSliced/s_sidebar/releases/tag/v1.0.0
