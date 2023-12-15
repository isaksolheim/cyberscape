# Cyberscape

A lively and fun Hugo theme for creating personal websites 🌐

![Screenshot](https://raw.githubusercontent.com/isaksolheim/cyberscape/main/images/screenshot.jpg)

💻 [Demo site](https://cyberscape.isak.me/)

🔨 [Demo site repo](https://github.com/isaksolheim/cyberspace)

## Overview

Cyberscape is designed to be a vibrant and engaging theme, perfect for those who enjoy the process of building personal websites.

## Install

To get started with Cyberscape, use the following command:

```
git submodule add https://github.com/isaksolheim/cyberscape themes/cyberscape
```

Then, open `config.toml` and add the following:

```
theme = "cyberscape"

# Enable this for tailwind in markdown files
[markup.goldmark.renderer]
unsafe=true

# Add menu links to things from /content/ here (eg. markdown.md)
[[menu.main]]
name = "markdown"
url = "/markdown/"
weight = 1
```

Navigate to the themes directory and install dependencies:

```
cd themes/cyberscape
npm i
```

## A Note on Tailwind

Cyberscape uses Tailwind CSS for styling. To ensure styles are up to date during development, run the following command from the themes directory:

```
npm run watch
```

This command will compile your Tailwind CSS as you make changes, keeping your development process smooth and streamlined.

The `tailwind.config.js` comes configured like the following:

```
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["content/**/*.md", "layouts/**/*.html", "../../content/**/*.md"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

If you wish to write Tailwind in any additional directories, add their relative path from the config file to the `content` field.

## Contributing

Feel free to contribute!

## License

[MIT](https://github.com/isaksolheim/cyberscape/blob/main/LICENSE)
