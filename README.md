# relative-goto
Visual Studio Code extension "relative-goto" allows you to jump to lines relative to the current line. Recommended to use together with the relative line settings in VS code.

## Features
- Jumps up and down in the same editor using relative line numbers as shown by relative line settings in vs code.
    - Positive numbers to jump down
    - Negative numbers to jump up
- Keeps the current character number when jumping
- On extension activation, change settings to ensure that lines numbers settings uses relative lines.
- Scroll / shift visible range to new position if the new position is out of visible range or if new position is the 'scrollOff' region.

## Requirements
<!-- If you have any requirements or dependencies, add a section describing those and how to install and configure them. -->
-- NIL

## Extension Settings
Any VS Code settings through the `contributes.configuration` extension point.  
This extension contributes the following settings:
* `relative-goto.enable`: enable/disable this extension

## Known Issues
<!-- Calling out known issues can help limit users opening duplicate issues against your extension. -->
-- NIL --

## Roadmap
- [ ] Add highlight to line on type before jumping to preview jump destination
- [ ] Bundle project to reduce size
- [ ] Optimize import to only impot what is needed from vs code lib
    - Use typings file for reference
    - e.g. use position.translate instead of creating a new position object
- [ ] Add settings to allow customization of jump style and default character position after jump

## Release Notes
### 0.3.0
- Updated range scrolling to only scroll/shift if the new position is out of visible range or in the scrollOff region.

### 0.2.0
- Setup function to ensure line numbers settings uses relative line numbers.

### 0.1.0
Initial release.

---
## License, Author and Contributing
This project is developed and made available under the "MIT License". Feel free to use it however you like!  
If you have any questions, contact us via via at tech@enkeldigital.com  
Authors:
- [JJ](https://github.com/Jaimeloeuf)