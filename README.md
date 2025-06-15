# Vite Plugin Bundle Styles 🎨

![GitHub Workflow Status](https://img.shields.io/github/workflow/status/AbdalrhmanCR7/vite-plugin-bundle-styles/CI?style=flat-square)
![npm](https://img.shields.io/npm/v/vite-plugin-bundle-styles?style=flat-square)
![License](https://img.shields.io/github/license/AbdalrhmanCR7/vite-plugin-bundle-styles?style=flat-square)

Welcome to the **Vite Plugin Bundle Styles** repository! This plugin bundles and compresses all your style files into a single optimized CSS file. With this tool, you can streamline your styling process, reduce load times, and improve the performance of your web applications.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Supported Preprocessors](#supported-preprocessors)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

## Features

- **Bundling**: Combines all your CSS files into one.
- **Compression**: Uses cssnano for optimized file size.
- **Support for Multiple Preprocessors**: Works with Sass, Less, Stylus, and more.
- **Easy Integration**: Simple setup with Vite.
- **Improved Performance**: Faster loading times for your applications.

## Installation

To install the plugin, run the following command in your project directory:

```bash
npm install vite-plugin-bundle-styles --save-dev
```

Or, if you prefer Yarn:

```bash
yarn add vite-plugin-bundle-styles --dev
```

## Usage

To use the plugin, you need to include it in your Vite configuration file (`vite.config.js`):

```javascript
import { defineConfig } from 'vite';
import bundleStyles from 'vite-plugin-bundle-styles';

export default defineConfig({
  plugins: [bundleStyles()],
});
```

This setup will automatically bundle and compress your styles during the build process.

## Configuration

You can customize the plugin's behavior through options in your Vite configuration. Here’s an example:

```javascript
export default defineConfig({
  plugins: [
    bundleStyles({
      output: 'dist/styles.css', // Specify output file name
      minify: true, // Enable or disable minification
      preprocessors: ['sass', 'less'], // Specify which preprocessors to use
    }),
  ],
});
```

### Options

- **output**: The path where the bundled CSS file will be saved.
- **minify**: A boolean to enable or disable CSS minification.
- **preprocessors**: An array of preprocessors you want to support.

## Supported Preprocessors

The plugin supports the following preprocessors:

- **Sass/SCSS**: Write styles using Sass syntax.
- **Less**: Use Less for advanced styling features.
- **Stylus**: Another option for writing CSS in a more dynamic way.
- **PostCSS**: Utilize PostCSS plugins for additional processing.

## Contributing

We welcome contributions! To get started:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test them.
4. Submit a pull request.

Please ensure your code follows the project's style guidelines and includes tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

To download the latest version of the plugin, visit the [Releases](https://github.com/AbdalrhmanCR7/vite-plugin-bundle-styles/releases) section. Here, you can find the latest updates and versions available for download.

To keep your project up to date, check the releases regularly for new features and improvements.

## Conclusion

The **Vite Plugin Bundle Styles** is a powerful tool for any developer looking to optimize their CSS workflow. By bundling and compressing styles, you can enhance your web application's performance and maintainability. 

Feel free to reach out if you have any questions or need assistance. We appreciate your interest in our project!

For more information and updates, don't forget to check the [Releases](https://github.com/AbdalrhmanCR7/vite-plugin-bundle-styles/releases) section.

---

Thank you for using **Vite Plugin Bundle Styles**! We hope it simplifies your styling process and enhances your development experience.