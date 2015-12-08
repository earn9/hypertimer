# History


## 2015-12-08, version 2.1.3

- Upgraded dependencies to the latest versions.


## 2015-07-13, version 2.1.2

- Fixed #1: Hypertimer crashed in case of multiple timeouts at the same time
  when running in paced mode.


## 2015-03-02, version 2.1.1

- Fixed replies not being send via socket.


## 2015-02-27, version 2.1.0

- Added support for ISOString dates for configuration of time, for using
  `setInterval`, and for `setTrigger`. The time returned from config is always
  an ISOString.
- Implemented a method `destroy`.
- Implemented events `'config'` and `'error'`.
- Implemented experimental support for synchronization between multiple
  hypertimers in a master/slave configuration.
- Fixed expanding all occurrences of intervals when changing the time
  to a moment in the future.
- Fixed expanding all occurrences of intervals started in the past.


## 2015-02-19, version 2.0.1

- Added missing development dependency `async` again.


## 2015-02-19, version 2.0.0

- Added a new option `paced: boolean` to distinguish running in paced mode
  or in unpaced (as fast as possible) mode. Option `rate` can now only be
  a number and is only applicable when `paced: true`.
- Removed method `setTime`, time can be configured on construction or with
  the function `config({time: ...})`.


## 2014-10-21, version 1.1.1

- Fixed `setTimeout` and `setTrigger` not working correctly when adding
  dates in the past or infinite delays. 
- Implemented a workaround for a bug in node.js v0.10.30 when calling `setTimeout`
  with a non-integer delay.


## 2014-07-22, version 1.1.0

- Added support for non-deterministic execution of events.


## 2014-07-17, version 1.0.0

- Implemented support for (async) discrete time.
- Removed support for negative rates.
- Added more docs and examples.


## 2014-07-15, version 0.1.0

- First functional release. Support for getting/setting time, and setting
  timeouts and intervals.


## 2014-07-11, version 0.0.1

- Library name reserved at npm and bower.
