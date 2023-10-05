# SetDPI

This is a sample and simple C++ console project to change windows Scale and Layout aka DPI scaling from command line parameters. It can work on single and multi-monitor setup.

## How to build (Windows 11)

- Download [VSCode](https://code.visualstudio.com/).

- Follow the tutorial [here](https://code.visualstudio.com/docs/cpp/config-msvc) to set up VSCode to compile C++ using the Microsoft Visual C++ compiler.

- In addition to the `C/C++` extension, also install the `C/C++ Extension Pack` extension.

- Close VSCode.

- Open, and I cannot emphasize this enough, the `Developer Command Prompt for VS 2022`, which you can run by searching for it in the Start menu.

- In that console window, type `code .`.

- In the VSCode window that opens, `Open Folder` and navigate to wherever you cloned this repository.

- Assure VSCode that I'm a perfectly aboveboard and trustworthy individual ;)

- Hit `Ctrl-Shift-B` to build, and you should see the `.exe` file appear in the top-level directory of the repository.

## How to use

It takes up to 2 parameters, first being the scale in percent. The second argument is the monitor index, which you get from windows display settings, if you click identify it shows you the index.

`SetDPI.exe [DPI scale value] [monitor index]`

If you have only one monitor or want only main monitor to change you can omit the monitor index.

To get the current scale of a monitor, replace the scale argument with `get` to print the current scaling. For automation with `value` only the scale is printed.

## Examples

- To set 2nd monitor to a scale value of 250
	- `SetDPI.exe 250 2`
- To set main monitor to a scale value of 125
	- `SetDPI.exe 125`
- To get the scale of the 2nd monitor
	- `SetDPI.exe get 2` prints `Current Resolution: 250`
	- `SetDPI.exe value 2` prints `250`

## Release

Get the release build and a sample AutoHotkey script with hotkey example from here https://github.com/imniko/SetDPI/releases/

## Credits

The whole credits go to @lihas of this project, https://github.com/lihas/windows-DPI-scaling-sample it was not possible without his findings.