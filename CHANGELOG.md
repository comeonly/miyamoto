# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased] - 2025-11-09

### Fixed
- Fixed typo in `actionOff` function (line 879): `vara` → `var data`
- Fixed typo in `actionCancelOff` function (line 891): `this.username` → `this.storage.get`
- Fixed missing `return` statement in `actionWhoIsIn` function (line 902-903)
- Fixed typo in `actionWhoIsOff` function (line 918): `this.age` → `this.storage`
- Fixed typo in `actionWhoIsOff` function (line 936): `telate` → `template`
- Fixed typo in `confirmSignIn` function (line 960): `isEmp` → `isEmpty`
- Fixed missing `&&` operator in `confirmSignOut` function (line 972)
- Fixed typo in Underscore.js library (line 996): `trray.prototype` → `r=Array.prototype`
- Fixed issue where sign-in/sign-out messages would repeat multiple times when updating the same time
  - Changed time comparison from millisecond precision to minute precision in `actionSignIn`
  - Changed time comparison from millisecond precision to minute precision in `actionSignOut`
  - This prevents duplicate messages when the same time is entered multiple times

### Changed
- Updated for compatibility with current Slack API specifications
