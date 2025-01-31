
# Changelog

## Unreleased

## 4.0.7 2019-10-28

- Add missing `heading` variant to `Heading` #754

## 4.0.6 2019-09-21

- Update dependencies
- Add layout package
- Add Slider and Switch to forms package

## 4.0.5 2019-08-21

- Fix publish

## 4.0.4 2019-08-21

- Add bundler setup & build for `@rebass/forms/styled-system`

## 4.0.3 2019-08-18

- Add forms package
- Update dependencies

## 4.0.2 2019-08-07
## 4.0.1 2019-08-06

- Fix ignore files
- Adjust build
- Update dependencies

## 4.0.0 2019-08-04

- New [`sx` prop](https://rebassjs.org/props/#sx-prop) for theme-based styles
- Use the `css` prop for un-themed, raw CSS values
- No additional Babel configuration required for the `sx` or `css` props
- Use the `sx` prop in MDX documents
- Built-in support for themeable component [variants](https://rebassjs.org/variants)
- Fully compatible with [Theme UI](https://theme-ui.com)

### Breaking Changes

- The default package now uses Emotion. To use Rebass with Styled Components, import the components from `rebass/styled-components` instead.
- The undocumented theme keys for `Box`, `Flex`, `Text`, `Heading`, `Link`, `Button`, `Image`, and `Card` are no longer supported. Use variants instead.
- The `@rebass/grid` package has been renamed (back to) `reflexbox`
- Heading: default `fontWeight` is now set to `heading`. Add styles to `theme.fontWeights` to customize the `heading` font weight.
- Button no longer supports the following props. Use the `sx` prop instead.
  `border`, `borderColor`, `borderWidth`, `borderStyle`, `borderRadius`, `borderTop`, `borderRight`, `borderBottom`, `borderLeft`, `borderX`, `borderY`
- Image no longer supports the following props. Use the `sx` prop instead.
  `border`, `borderColor`, `borderWidth`, `borderStyle`, `borderRadius`, `borderTop`, `borderRight`, `borderBottom`, `borderLeft`, `borderX`, `borderY`
- Link no longer includes default styles. Add styles to `theme.variants.link` to customize link styles.
- Card no longer supports the following props. Use the `sx` prop instead.
  `border`, `borderColor`, `borderWidth`, `borderStyle`, `borderRadius`, `borderTop`, `borderRight`, `borderBottom`, `borderLeft`, `borderX`, `borderY`, `boxShadow`, `textShadow`, `background`, `backgroundImage`, `backgroundSize`, `backgroundPosition`, `backgroundRepeat`,


## [3.1.0] 2019-03-23

- Update to Styled System v4

## [3.0.1] 2019-01-18

- Update styled-system #555

## [3.0.0] 2018-12-01

- Reduced package size
- Reduced number of components to 8
- Updated for Styled Components v4 and Emotion v10
- Reduced dependencies
- Removed default theme and colors
- Removed Provider component
- Added variant theme support for Button and Card components
- Removed `is` prop in favor of Styled Components' and Emotion's `as` prop
- Uses Box component as base for all other components
- Removed `css` prop in favor of Styled Components' and Emotion's implementations

## [3.0.0-12] 2018-11-29

- Removes `css` prop in favor of babel-plugin-styled-components
- Adds build setup for Emotion 10

## [3.0.0-11] 2018-11-13

- Update dependencies

## [3.0.0-10] 2018-11-12

- Sets `box-sizing: border-box` on base Box component

## [3.0.0-9] 2018-09-22

- Adds flexbox props back to Box component

## [3.0.0-6] 2018-09-13

- Adds emotion package

## [3.0.0-2] 2018-09-11

- Update styled-system
- Update docs

## [3.0.0-1] 2018-09-10

- Update docs for v3

## [3.0.0-0] 2018-09-08

- Smaller package
- Reduced number of components to 8
- Upgraded for styled-components v4
- Reduced dependencies to one
- Removed default theme and colors
- Removed Rebass Provider component
- Added variant theme support to Button and Card
- Removed `is` prop in favor of styled-components `as` prop
- Uses Box component as the base for all other components

## [2.3.2] 2018-09-08

- Update repo in package.json
- Update readme

## [2.3.1] 2018-09-08

- Fix bad prepublish build

## [2.3.0] 2018-09-08

- Upgrade to @rebass/components, @rebass/grid, and styled-system v3

## [2.2.0] 2018-09-08

- Use `polished` for color manipulation instead of `chroma-js`

## [2.1.1] 2018-09-08

- Support `width` prop on Card
- Update docs

## [2.1.0] 2018-08-14

- Add Hide component

## [2.0.1] 2018-06-30

- Add `fontFamily` to Heading and Text components
- Update docs

## [2.0.0] 2018-06-24

### Added

- Support for [emotion][emotion]

### Changed

- [styled-system](https://github.com/jxnblk/styled-system) v2
- [grid-styled](https://github.com/jxnblk/grid-styled) v4
- Moves components to separate modules
- Uses [system-components](https://github.com/jxnblk/styled-system/tree/master/system-components)
- Updates docs site

#### Breaking

- Renamed components
  - TabItem -> Tab
  - DotButton -> Dot
  - PanelHeader -> Panel.Header
  - PanelFooter -> Panel.Footer
- Default theme (changed to match styled-system)
  - The `colors` object no longer uses Palx
  - Array color values have been removed
  - `radius` has been replaced with `radii`
  - `font` has been replaced with `fonts`
  - `monospace` has been removed
  - Theme fields are no longer exposed as exports
- Props
  - `width` is only available on Flex and Box
  - `fontSize` is only available on typographic components
  - `direction` is now `flexDirection`
  - Flex `align` is now `alignItems`
  - Flex `justify` is now `justifyContent`
  - Flex `wrap` is now `flexWrap`
  - Arrow `up` is now `direction='up'`
  - `active` props have been removed in favor of custom styles
  - Border now uses [styled-system border props](https://github.com/jxnblk/styled-system#borders)
  - Banner `image` is now `backgroundImage`
  - Absolute, Fixed, Relative, and Sticky now require values for `top`, `right`, `bottom`, and `left` props
  - Drawer `position` prop has been renamed to `side`
  - Drawer `size` prop has been replaced with `width` and `height` props

### Removed

- Custom HOC `hoc`
- `createLibrary` function
- `util`
- `createComponent`
- Palx dependency
- ScrollCarousel component
- CarouselSlide component
- Star comonent


[emotion]: https://github.com/emotion-js/emotion
