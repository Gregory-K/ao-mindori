# ao mindori

A blue-green theme and colour scheme for Sublime Text 4.

Version: 0.1.261014alpha


## Contents

Themes:

- **ao-mindori Dark**, the main theme.
- **ao-mindori Adaptive**, Dark with Adaptive's themed title bar: the menu goes under a burger button and the title bar, tab bar and UI take their colour from the colour scheme's background. Only dark colour schemes are supported, for now.

Colour schemes: **ao-mindori** and **ao-mindori-alt**.

Each theme has its own `Widget - <theme>` settings and widget colour scheme, for input fields and panels.


## Install

Open 'Packages' directory with  
`Ctrl+Shift+P` (`Cmd+` for MacOS) > `Preferences: Browse Packages`.

Download `ao-mindori-v<version>.zip` from the [latest release](https://github.com/Gregory-K/ao-mindori/releases/latest) and extract it there.

OR clone the repository into the 'Packages' directory:

```sh
git clone https://github.com/Gregory-K/ao-mindori.git
```

> Note: The package's directory must be named `ao-mindori`.


## Setup

In `Preferences.sublime-settings`:

```json
"theme": "ao-mindori Dark.sublime-theme",
"color_scheme": "ao-mindori.sublime-color-scheme",
```


## File icons

Shipped as a file icon theme, `icons/<theme>.sublime-file-icons`, which maps file extensions and names to icons. It needs Sublime Text 4206+ and loads only with the theme of the same name, hence one identical copy per theme.

C headers and Fortran stay scope based (`preferences/`), since an extension can't tell C from C++ headers or fixed-form from free-form Fortran. The Fortran icons need a Fortran syntax package.


## Layout

- `common/`, `adaptive/`, `fallback/`: a full copy of the Default theme's textures, kept to restyle any element. The themes reference the ones they use by path.
- `extras/`: our own textures.
- `icons/`: the file icons, their mapping and the icon licences.
- `preferences/`: the scope based icons.


## Credits

- File icons from [A File Icon](https://github.com/SublimeText/AFileIcon) (MIT), and the go gopher, cheader, xml, procfile, imageunsupported and Fortran icons from [FileIcons](https://github.com/braver/FileIcons) (MIT).  
See `icons/LICENSE.txt`.
- Textures from Sublime Text's Default theme.


## License

Copyright (c) 2024 Gregory.K

Mozilla Public License 2.0, see [License.txt](License.txt).  
Except the file icons (MIT, see `icons/LICENSE.txt`) and the Default theme textures, which belong to Sublime HQ.
