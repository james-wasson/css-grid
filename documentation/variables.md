# Grid Variables

## Gap

Gap is defined by the variable `$grid-gap` and is initally `1.5rem`

Gap can be futher broken up into `$grid-column-gap` and `$grid-row-gap` defining the column and row gap respectively and are initally set to be equal to `$grid-gap`

Please see the [Gap](./gap.md) documentation page for modifiers.

## Resizeable Grids

Grids can be specified to not be resizeable by setting the `$grid-resizeable` variable to `false`

This can be further broken up into `$grid-columns-resizeable` and `$grid-rows-resizeable` both of which are initally set to the value of `$grid-resizeable`

This affects the ability to resize the grid but does not affect positioning.

Read more here: [Columns and Rows](./columns-rows.md)

## Row and Column Counts

Supported row and column counts are defined by `$grid-column-row-count` and is initally set to `20`

This can be further broken up into `$grid-column-count` and `$grid-row-count` both of which are initally set to the value of `$grid-column-row-count`

This limits [Column and Row](./columns-rows.md) resizing and [Positioning](./positioning.md) to within max column and row counts.

**Note:** Increasing this value has a large affect on file size and should be kept at a fairly low value.

## Breakpoints

You can enable/disable breakpoints by setting the `$grid-breakpoints-enabled` variable which is initally set to `true`

This can be further broken down into:
- `$grid-mobile-enabled`
- `$grid-tablet-enabled`
- `$grid-touch-enabled`
- `$grid-desktop-enabled`
- `$grid-widescreen-enabled`
- `$grid-fullhd-enabled`

All of the above are set to `$grid-breakpoints-enabled` unless otherwise specified

## Nesting

You can specify the supported nesting count of the grid by increaing the value of `$grid-nesting-count` which is initally set to `0`

Read more here: [Nested Grids](./nested-grids)

# Bulma Variables

We pull in a few variables from Bulma to maintain compatibility. The documentation for these variables is located [here](https://bulma.io/documentation/customize/variables/).

**Note:** This library can be used without Bulma. These variables are set in our library as well as Bulma.

We pull in the breapoint variables that will be updated as bulma is:
- `$gap`
- `$tablet`
- `$desktop`
- `$widescreen`
- `$fullhd`

Other variables:
- `$navbar-height` - [docs here](https://bulma.io/documentation/components/navbar/#variables)

Current Bulma defintions:
- `$gap` = `32px`
- `$tablet` = `769px`
- `$desktop` = `960px + (2 * $gap)`
- `$widescreen` = `1152px + (2 * $gap)`
- `$fullhd` = `1344px + (2 * $gap)`
- `$navbar-height` = `3.25rem`
