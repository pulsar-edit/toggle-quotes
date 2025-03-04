# Toggle Quotes

Toggle a single-quoted string to a double-quoted string, and vice versa.

![toggle-quotes-demo](https://cloud.githubusercontent.com/assets/823545/9016150/aa73ab62-379c-11e5-8622-8dbb492ff4f1.gif)

This is a package for [Pulsar](https://pulsar-edit.dev/), a community-led hyper-hackable text editor.

## Usage

Place the cursor within a string and execute the `Toggle Quotes: Toggle` command to toggle that string between single and double quotes. Only available when using a grammar that supports single-quoted and double-quoted strings, or any other configured string character (e.g. JavaScript, Python, Ruby, etc.).

### Commands

Command                | Description
-----------------------|--------------
`toggle-quotes:toggle` | Toggles the quote characters used for quoted strings between the configured `Quote Characters` (`'` and `"` by default).

### Keybindings

Command            | Linux  | OS X  | Windows
-------------------|--------|-------|----------
`toggle-quotes:toggle` | <kbd>Ctrl-"</kbd> | <kbd>Cmd-"</kbd> | <kbd>Ctrl-"</kbd>

Custom keybindings can be added by referencing the above commands.  To learn more, visit the [Using Atom: Basic Customization](https://atom.io/docs/latest/using-atom-basic-customization#customizing-key-bindings) or [Behind Atom: Keymaps In-Depth](https://atom.io/docs/latest/behind-atom-keymaps-in-depth) sections in the flight manual.

### Configuration

Configuration Key Path      | Type | Default | Description
----------------------------|------|---------|------------
`toggle-quotes.quoteCharacters` | `string` | `'"` | The characters `toggle-quotes:toggle` toggles between. No whitespace.

You can add [language-specific settings](http://flight-manual.atom.io/using-atom/sections/basic-customization/#language-specific-configuration-settings) for languages with more exotic string delimiters. For example, this setting in your `config.cson` will add backticks in JavaScript files, but not in other kinds of files:

```cson
".js.source":
  "toggle-quotes":
    quoteCharacters: "\"'`"
```

## Contributing

Always feel free to help out!  Whether it's filing bugs and feature requests
or working on some of the open issues, Atom's [contributing guide](https://github.com/atom/atom/blob/master/CONTRIBUTING.md)
will help get you started while the [guide for contributing to packages](https://github.com/atom/atom/blob/master/docs/contributing-to-packages.md)
has some extra information.

## License

[MIT License](http://opensource.org/licenses/MIT) - see the [LICENSE](https://github.com/pulsar-edit/toggle-quotes/blob/master/LICENSE.md) for more details.
