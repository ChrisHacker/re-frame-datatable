# Change Log
All notable changes to this project will be documented in this file. This change log follows the conventions of [keepachangelog.com](http://keepachangelog.com/).

## [0.5.1] - 2017-01-17
### Added
- ::column-label became optional
- ::column-label can now accept either string as before or an arbitrary Reagent component
- New option: ::header-enabled? which can be used to prevent DataTable from <thead> rendering
- "sortable" columns are marked with special class for styling via CSS

## [0.5.0] - 2016-12-30
### Breaking
- Pagination controls are not rendered by default, extracted into separate component

### Added
- Ability to create own pagination controls
- Callback to unselect all rows in DataTable
- Customizable rendering of empty DataTable

### Fixed
- Empty DataTable doesn't select "selected all" checkbox
- Default pagination control works correctly with empty DataTable

## [0.4.0] - 2016-12-27
### Added
- Support for optional extra row inside `<thead>` via `::extra-header-row-component`
- Support for optional `<tfoot>` via `::footer-component`
- Ability to inject arbitrary classes into rendered `<td>` and `<tr>` elements
- Bumped [re-frame](https://github.com/Day8/re-frame) version to 0.9.1

## [0.3.0] - 2016-12-21
### Added
- Selection of rows (including a subscription to selected elements)

### Changed
- Changed all datatable-related keywords to namespace-qualified keywords

## [0.2.0] - 2016-12-19
### Added
- Switched to [re-frame](https://github.com/Day8/re-frame) 0.9.0
- `::render-fn` key that allows to specify custom rendering function
- Styling of `<th>` element after sorting

### Removed
- `::th-classes` key from `columns-def` vector elements. Styling should happen outside of component

## 0.1.0 - 2016-12-15
### Added
- Initial DataTable implmenetation
- sorting
- pagination
- Styling of `<table>` element
