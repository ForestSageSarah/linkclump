# Linkclump 
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/9e38a24d7f524c6ca73c07e8948d58a7)](https://www.codacy.com/manual/benblack86/linkclump?utm_source=github.com&utm_medium=referral&utm_content=benblack86/linkclump&utm_campaign=Badge_Grade) [![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) 

## Table of Contents 
- [About The Project](#about-the-project)
- [Key Features](#key-features)
- [Getting Started](#getting-started)
- [Installation](#installation) 
- [Prerequisites](#prerequisites) 
- [Build Instructions](#build-instructions) 
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## About The Project 
Linkclump is a Chrome extension that allows you to quickly open, copy, or bookmark multiple links from any webpage using a simple drag-selection tool. With a focus on efficiency and ease of use, Linkclump helps streamline your workflow by enabling rapid link management. This project is a fork of the original extension by the original author. It has been updated for modern browsers with enhanced functionality and compatibility under Manifest V3 while preserving its core purpose. 

### Key Features 
- **Multiple Actions:** Open links in new tabs or windows, copy them to your clipboard, or add them to your bookmarks. 
- **Drag-Selection Interface:** Easily select multiple hyperlinks with a simple click-and-drag mechanism. 
- **Customizable Options:** Configure key bindings and behavior to match your workflow.
- **Enhanced Compatibility:** Updated for Manifest V3 and modern Chrome browsers.

## Getting Started 

### Installation 
Install Linkclump from the [Chrome Web Store](https://chrome.google.com/webstore/detail/linkclump/lfpjkncokllnfokkgpkobnkbkmelfefj). 

### Prerequisites 
For end users, no additional setup is needed. 

For developers looking to build or modify Linkclump, ensure you have: 
- [Node.js](https://nodejs.org/) (if modifying build scripts)
- [Apache Ant](https://ant.apache.org/) (for building the extension)

### Build Instructions 
Linkclump uses Apache Ant for its build process. To build the extension, run: 

```sh ant ``` 

Alternatively, you can build using Docker with:

```sh docker run --mount type=bind,source="$(pwd)",target=/app frekele/ant:1.10.3-jdk8u111 ant -f /app/build.xml ``` 

This process runs tests and creates a zip file ready for upload to the Chrome Web Store. 

## Usage 
After installation, navigate to any webpage, press the configured key (default is **Z** with left-click), and drag to select multiple links. Upon releasing the mouse button, Linkclump will perform your chosen action—opening links in new tabs or windows, copying them in your preferred format, or bookmarking them. 

## Contributing 
Contributions are welcome! If you have suggestions or improvements, please fork the repository and submit a pull request. For major changes, consider opening an issue first to discuss your ideas. 

## License 
This project is licensed under the MIT License. Please view the [LICENSE](LICENSE) file for details. 

## Acknowledgments 
- **Original Author:** Thanks to the original author for creating the foundation for Linkclump.
- **Codacy:** For code quality and continuous integration insights.
- **The Open Source Community:** For valuable feedback and contributions.
