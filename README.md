# meiyo_styles

---

This is **`meiyo_styles`**, an SCSS style package developed to provide a consistent base and a set of reusable visual components for my web projects. Inspired by the concept of having full control over design, this package avoids bulky CSS frameworks, focusing on flexibility and complete customization through the power of SCSS.

## Features

* **Modular and Organized:** Styles are divided into logical modules (base, components, layout, mixins) for easy navigation and maintenance.
* **Reusable:** Simply install via NPM and import into any new project.
* **Compilable:** Includes scripts to compile your SCSS to CSS.

---

## Installation

To include `meiyo_styles` in your project, install it via npm:

```bash
npm install meiyo_styles
````

-----

## Usage

After installation, you can import the styles directly into your project's main SCSS file. The Sass compiler will handle finding the files within the `node_modules` folder.

### Importing into your SCSS

```scss
// Example: your-project/src/styles/main.scss

// Imports all main styles from the package
@import 'meiyo_styles';

// Optional: You can also import specific files from the package if needed
// For example, to access only its variables or mixins
@import 'meiyo_styles/src/base/variables';
@import 'meiyo_styles/src/mixins/responsive';

/*
  Add your project-specific styles here,
  or override 'meiyo_styles' if necessary.
*/
body {
  font-family: var(--font-primary, sans-serif);
  color: #333;
}
```

### Compilation Configuration Example (with Sass)

The `npm install` command already includes the compiled CSS ready for use, but if you want to compile the SCSS from your repository for any reason, ensure your project has an SCSS compilation script configured, like this in your main `package.json`:

```json
// your-project/package.json
{
  "name": "your-project",
  // ...
  "scripts": {
    "sass:build": "sass src/styles/main.scss:public/css/styles.css",
    "sass:watch": "sass --watch src/styles/main.scss:public/css/styles.css"
  },
  "devDependencies": {
    "sass": "^1.x.x"
  }
}
```

-----

## Package Structure

The internal structure of `meiyo_styles` is organized as follows:

```
meiyo_styles/
├── src/
│   ├── base/               # Fundamental styles (reset, typography, variables)
│   ├── components/         # Reusable UI components (buttons, cards, forms)
│   ├── layout/             # Layout structure and organization (header, footer, grid)
│   ├── utilities/          # Reusable and utility SCSS mixins, variables, and functions
│   └── main.scss           # Main entry point for the package
├── package.json
└── README.md
```

-----

## Development (For Contributors)

If you are developing or contributing to `meiyo_styles` directly:

1.  Clone this repository:
    ```bash
    git clone [https://github.com/blink992/meiyo_styles.git](https://github.com/blink992/meiyo_styles.git)
    cd meiyo_styles
    ```
2.  Install development dependencies:
    ```bash
    npm install
    ```

-----

## License

This project is licensed under the **MIT** license. See the [LICENSE](https://www.google.com/search?q=./LICENSE.md) file for more details.

-----

## Contact

Pedro Arthur Gregorio Abreu - [pedro.agb2004@gmail.com](mailto:pedro.agb2004@gmail.com)

Project Link: [https://github.com/meiyo-aru/meiyo-styles](https://github.com/meiyo-aru/meiyo-styles)

-----
