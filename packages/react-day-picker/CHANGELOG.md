# Changelog

### v8.1.4

- fix: use parsed `fromDate`/`toDate` in `useInput` by @hypergeometric in [#1524](https://github.com/gpbl/react-day-picker/pull/1524)
- changed: add names to fields and buttons by [@gpbl](https://github.com/gpbl) in [#1530](https://github.com/gpbl/react-day-picker/pull/1530)
- changed: focus vs focus-visible styles by [@gpbl](https://github.com/gpbl) in [#1531](https://github.com/gpbl/react-day-picker/pull/1531)

### v8.1.3

- fix: `onDayClick` called twice in selection mode, by [@gpbl](https://github.com/gpbl) in [#1520](https://github.com/gpbl/react-day-picker/pull/1520)
- changed: accept `undefined` for the modifier props, by [@gpbl](https://github.com/gpbl) in [#1521](https://github.com/gpbl/react-day-picker/pull/1521)

### v8.1.2

- fix: do not focus disabled or hidden days, by [@gpbl](https://github.com/gpbl) in [#1519](https://github.com/gpbl/react-day-picker/pull/1519)

### v8.1.1

- fix: prevent focus from moving beyond `toDate` and `fromDate`, by [@kimamula](https://github.com/kimamula) in [#1468](https://github.com/gpbl/react-day-picker/pull/1468)
- fix: page keys not working when using `setMonth`, by [@kimamula](https://github.com/kimamula) in [#1510](https://github.com/gpbl/react-day-picker/pull/1510)
- fix: add `onSelect` to the `DayPickerContextValue`, by [@gpbl](https://github.com/gpbl) in [#1515](https://github.com/gpbl/react-day-picker/pull/1515)
- fix: `rdp` class not added to root element when using `className` prop, by [@gpbl](https://github.com/gpbl) in [#1517](https://github.com/gpbl/react-day-picker/pull/1517)

## v8.1.0

- new: add prefix to auto generated ids, by [@mihkeleidast](https://github.com/mihkeleidast) in [#1493](https://github.com/gpbl/react-day-picker/pull/1493)
- new: `addedToRange` to the exported utilities, by [@stopr29](https://github.com/stopr29) in [#1495](https://github.com/gpbl/react-day-picker/pull/1495)
- new: revert to use disabled attribute instead of `aria-disabled` (reverts, by [@gpbl](https://github.com/gpbl) in [#1451](https://github.com/gpbl/react-day-picker/pull/1451))See ongoing discussion in [#1468](https://github.com/gpbl/react-day-picker/pull/1468)
- new(css): use pure selector for CSS variables, by [@andyschulzz](https://github.com/andyschulzz) in [#1481](https://github.com/gpbl/react-day-picker/pull/1481), [#1499](https://github.com/gpbl/react-day-picker/pull/1499)
- fix: `@reach/auto-id` warnings, by removing the dependency, by [@gpbl](https://github.com/gpbl) in [#1484](https://github.com/gpbl/react-day-picker/pull/1484)
- fix: home/end buttons behavior with `startOfWeek`, by [@apdrsn](https://github.com/apdrsn) in [#1492](https://github.com/gpbl/react-day-picker/pull/1492)
- package: upgraded dependencies, by [@gpbl](https://github.com/gpbl) in [#1497](https://github.com/gpbl/react-day-picker/pull/1497)

### v8.0.7

- fixed: missing `dropdown_year` CSS class in `YearsDropdown`, by [@pwolfert](https://github.com/pwolfert) in [#1466](https://github.com/gpbl/react-day-picker/pull/1466)
- fixed: Maximum update depth exceeded when select the range date, by [@gpbl](https://github.com/gpbl) in [#1470](https://github.com/gpbl/react-day-picker/pull/1470)

### v8.0.6

- fixed: exclude internal modifiers from the `styles` props (`modifiersStyles` should be used instead), by [@gpbl](https://github.com/gpbl) in e1449eaa
- fixed: better typings for the props returned by `useInput`, by [@gpbl](https://github.com/gpbl) in 3ea6728b

In the rare cases you are using an invalid key to the `styles` prop, you may get type errors when upgrading to this release. Just remove the invalid lines from the value of `styles`, as they weren't working anyway. See issue [#1464](https://github.com/gpbl/react-day-picker/issues/1464).

### v8.0.5

- changed: use `aria-disabled` instead of `disabled` attribute in buttons ([#1451](https://github.com/gpbl/react-day-picker/pull/1451))
- fixed: focus navigation breaks with disabled days ([#1451](https://github.com/gpbl/react-day-picker/pull/1451))

### v8.0.4

- changed: add src directory to the package for better source maps

### v8.0.3

- fix: `toMonth` prop to include the full month ([#1429](https://github.com/gpbl/react-day-picker/pull/1429))
- changed: better date-fns import should improve tree-shaking ([#1436](https://github.com/gpbl/react-day-picker/pull/1436))
- changed: removed `browser` entry in `package.json` ([#1436](https://github.com/gpbl/react-day-picker/pull/1436))

### v8.0.2

- new: added `weekStartsOn` prop ([#1422](https://github.com/gpbl/react-day-picker/pull/1422))
- new: split the `Caption` components into `CaptionDropdowns` and `CaptionNavigation` components. This change should make easier to customize the caption. ([#1426](https://github.com/gpbl/react-day-picker/pull/1426))

### v8.0.1

- changed: added React 18 to the peer dependencies

## v8.0

This version introduces breaking changes and it is mostly incompatible with v7. See the [redesigned website](https://react-day-picker.js.org) for more details.

### Notable changes

- native TypeScript support
- selection modes: single, multiple, range
- added [date-fns](http://date-fns.org) library as peer dependecy
- replaced `DayPickerInput` component with `useInput` hook
- improved ARIA support

See also: ➡️ **[Upgrading from v7](https://react-day-picker.js.org/guides/upgrading)**.

---

## Older changelog

See [/v7/CHANGELOG.md](https://github.com/gpbl/react-day-picker/blob/v7/CHANGELOG.md) for the changelog of versions before 8.
