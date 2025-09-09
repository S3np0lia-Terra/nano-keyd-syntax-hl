# GNU Nano Syntax Highlighting for Keyd Configuration Files

----------

This repository provides a comprehensive syntax highlighting file for GNU Nano,
designed primarily for configuration files of the Keyd remapping daemon.
The rules can also be useful for other configuration files with an '.ini'- or
'.conf'-like structure. Some rules for '.ini' and '.conf' files are already 
active in the syntax file. Lines that could conflict with Keyd-specific highlighting
are commented out by default. Instructions for enabling or adjusting these rules are
included directly in the file as comments, allowing you to safely adapt the higlighting
for other configuration files while keeping Keyd highlighting rules intact.

----------

## 🖥️  *How does it look?*
| Highlighting disabled | Highlighting enabled
| :-------------: | :--------------: |
| ![Highlighting disabled](./examples/without_highlighting.png)  | ![Highlighting enabled](./examples/with_highlighting.png)  |

----------

## 🎨 *What does each color represent?*
### Highlighting of global options and device lists
- ![latte color](https://placehold.co/15x15/af875f/transparent) Latte: Comments;
- ![sky color](https://placehold.co/15x15/87afff/transparent) Sky: `include` directives;
- ![yellow color](https://placehold.co/15x15/yellow/transparent) Yellow: Listed device IDs;
- ![sage color](https://placehold.co/15x15/87af5f/transparent) Sage: Paths and filenames after `include`;
- ![lagoon color](https://placehold.co/15x15/00afd7/transparent) Lagoon: The [global] section and its options;
- ![crimson color](https://placehold.co/15x15/crimson/transparent) Crimson: Invalid syntax;
### Highlighting of functional configuration and remapping rules
- ![orange color](https://placehold.co/15x15/orange/transparent) Orange: Key area (left to the equal sign);
- ![sand color](https://placehold.co/15x15/d7d787/transparent) Sand: Value area (right to the equal sign)
- ![red color](https://placehold.co/15x15/red/transparent) Red: 
    1. The [ids] section wildcard;
    2. Blacklisted devices, e.g. `-1234:1234`;
    3. The assignment operator `=`;
- ![sea color](https://placehold.co/15x15/0087d7/transparent) Sea: Numeric digits;
- ![ocher color](https://placehold.co/15x15/afaf00/transparent) Ocher: Parentheses and their content;
- ![lightyellow color](https://placehold.co/15x15/fabd2f/transparent) LightYellow: String values;
- ![brick color](https://placehold.co/15x15/d75f00/transparent) Brick: Functions;
- ![lime color](https://placehold.co/15x15/afd700/transparent) Lime: 
    1. Macros and modifiers;
    2. Section headers;
- ![teal color](https://placehold.co/15x15/00af5f/transparent) Teal: Section headers with modifiers, e.g. `[nav:S]`;

----------

## Optional Highlighting for Extended Config Syntax
In addition to the Keyd-specific syntax, this higlighting file also supports some **optional constructs** that are common in '.ini'
or '.conf' files, but not currently used by Keyd.
These include:

- Numeric values with optional suffixes: 'ms', 's', 'us' (suffixes inherit the color of the preceding number);
- ![lagoon color](https://placehold.co/15x15/00afd7/transparent) Lagoon: Floating-point numbers;
- ![beet color](https://placehold.co/15x15/af00af/transparent) Beet: Boolean values ('true' / 'false');

These rules are included to make the syntax file more versatile for other configuration files and can safely be ignored
if you are only working with Keyd configs.

----------

## Acknowledgements
- [Keyd](https://github.com/rvaiya/keyd) project by rvaiya.

----------

## License
[MIT](./LICENSE) 
