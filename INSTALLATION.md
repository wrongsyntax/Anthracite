# `themer`

Your theme's unique URL:

https://themer.dev/?colors.dark.shade0=%23292c33&colors.dark.shade7=%23c3c3c3&colors.dark.accent0=%23cc241d&colors.dark.accent2=%23d79921&colors.dark.accent3=%2371981a&colors.dark.accent4=%23689d6a&colors.dark.accent5=%23458588&colors.dark.accent6=%2315d186&colors.dark.accent7=%23b86393&colors.dark.accent1=&colors.dark.shade3=%230ba56a&colors.dark.shade5=%23c3c3c3&colors.dark.shade4=&colors.dark.shade1=%231e2126&colors.dark.shade6=%23ebdbb2&colors.dark.shade2=%231e2126&calculateIntermediaryShades.dark=false

If you find `themer` useful, here are some ways to support the project:

* Star [`themer` on GitHub](https://github.com/mjswensen/themer)
* Follow [@themerdev](https://twitter.com/themerdev) on Twitter
* [Send a tip through the Brave Browser](https://brave.com/the537), either on [the repository page](https://github.com/mjswensen/themer) or [the Web UI](https://themer.dev)
* Pay what you want when downloading your theme from [themer.dev](https://themer.dev)

# Installation instructions

## Atom Syntax

Use the `apm link` command to install the generated theme package to Atom:

    apm link 'Atom Syntax/themer-dark-syntax'

Then open/reload Atom and select the desired theme in the list of available syntax themes.

## Atom UI

Use the `apm link` command to install the generated theme package to Atom:

    apm link 'Atom UI/themer-dark-ui'

Then open/reload Atom and select the desired theme in the list of available UI themes.

## Chrome

1. Launch Chrome and go to `chrome://extensions`.
2. Check the "Developer mode" checkbox at the top.
3. Click the "Load unpacked extension..." button and choose the desired theme directory (`Chrome/Themer Dark`).

(To reset or remove the theme, visit `chrome://settings` and click "Reset to Default" in the "Appearance" section.)

## CSS

Import the generated theme file into your stylesheet via `@import()`, or into your HTML markup via `<link>`.

`hex.css` provides the theme colors in hex format; `rgb.css` and `hsl.css` in RGB and HSL formats respectively along with individual channel values for further manipulation if desired.

Generated files:

* `CSS/hex.css`
* `CSS/rgb.css`
* `CSS/hsl.css`

## Firefox Add-on

To use the generated extension package, the code will need to be packaged up and signed by Mozilla.

To package the code in preparation for submission, the `web-ext` tool can be used:

    npx web-ext build --source-dir 'Firefox Add-on/Themer Dark'

Then the package can be submitted to Mozilla for review in the [Add-on Developer Hub](https://addons.mozilla.org/en-US/developers/addon/submit/distribution).

Learn more about Firefox themes from [extensionworkshop.com](https://extensionworkshop.com/documentation/themes/)

To theme Firefox without the need to create a developer account and go through the extension review process, see themer's integration with [Firefox Color](https://color.firefox.com).

## Firefox Color

The Firefox Color add-on allows for simple theming without the need for a developer account or package review process by Mozilla.

1. Install the [Firefox Color add-on](https://addons.mozilla.org/en-US/firefox/addon/firefox-color/).
2. Open 'Firefox Color/themer-dark.url' directly with Firefox.
3. Click "Yep" when prompted to apply the custom theme.

For a more fully featured Firefox theme, see themer's Firefox theme add-on generator.

## iTerm

1. Launch iTerm
2. Press `command`-`I` to open the iTerm preferences
3. Choose Colors > Color Presets... > Import... and choose the generated theme file (`iTerm/themer-iterm-dark.itermcolors`)

## Xcode

Copy (or symlink) the generated theme file to Xcode's themes directory:

    mkdir -p ~/Library/Developer/Xcode/UserData/FontAndColorThemes
    cp 'Xcode/Themer Dark.dvtcolortheme' ~/Library/Developer/Xcode/UserData/FontAndColorThemes/

Then restart Xcode. The theme will be available in Preferences > Fonts and Colors.