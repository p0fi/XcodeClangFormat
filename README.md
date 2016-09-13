# XcodeClangFormat

### [⚙ Download Latest Release](https://github.com/mapbox/XcodeClangFormat/releases/latest)

This plugin written for Xcode 8's new plugin infrastructure uses Clang's `libclangFormat` library to format code according to a `.clang-format` file.

Open the app, select a predefined style, or open the `.clang-format` file from your project:

![](screenshot-config.png)

Then, use the <kbd>Format Source Code</kbd> command in Xcode's <kbd>Editor</kbd> menu:

![](screenshot-format.png)

Due to macOS Sandboxing restrictions, this Plugin behaves slightly differently compared to the command line `clang-format` command: It always uses the style selected in the configuration app, and will not use the nearest `.clang-format` file on disk.

### Building

To build XcodeClangFormat, run `./configure` on the command line, then build the XcodeClangFormat scheme in the included Xcode project.