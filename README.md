# run-react-native [![NPM version][npm-image]][npm-url] [![Downloads][downloads-image]][npm-url] [![Gitter chat][gitter-image]][gitter-url]
> Simplify react-native development

If you've worked with `react-native` then you know how tedious it is to:

* Start the packager
* Start an emulator
* Install the build on the emulator

Sometimes you also need to do things like:

* Re-install the apk
* Re-start the packager

Do you have these open in separate terminal windows?

`run-react-native` is an interactive bash script that encapsulates all these
commands for you and more so you can have only 1 terminal open and speed up your
development cycle.

## Installation

`npm i -g run-react-native`

Before you can run it you'll need to do a few things:

* Ensure `emulator` and `adb` are available in your `$PATH`.
* `cd $YOUR_PROJECT`
* Add `export RUN_REACT_NATIVE_ANDROID_AVD='name-of-my-development-avd'`.  You can get the names of available avds on your system by running `emulator -list-avds`.

## Example

In this screencast, I'll demonstrate `run-react-native` in action.

![Screencast of run-react-native being used in a terminal window](./cast.gif?raw=true "Screencast of run-react-native being used in a terminal window")

### tl;dw

After the packager and emulator start:

* the apk is installed you then have the following commands available:
  * h, help - Prints this menu to stdout.
  * ke      - Kills the emulator.
  * ra      - Reinstalls the apk on the emulator.
  * rap     - Reloads the app on the emulator.
  * re      - Reloads the emulator.
  * rp      - Reloads the packager.
* Pressing `CTRL-C` exits the process and all child processes are killed.

## TODO

- [ ] Add support for iOS


## LICENSE
``````
The MIT License (MIT)

Copyright (c) 2016 Kogo Software LLC

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
``````

[downloads-image]: http://img.shields.io/npm/dm/run-react-native.svg
[npm-url]: https://npmjs.org/package/run-react-native
[npm-image]: http://img.shields.io/npm/v/run-react-native.svg

[gitter-url]: https://gitter.im/kogosoftwarellc/run-react-native
[gitter-image]: https://badges.gitter.im/kogosoftwarellc/run-react-native.png
