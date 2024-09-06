# Shortcuts-for-ARC-Browser
A Chrome Extension Generator, that creates simple chrome extensions to act like bookmarks/ shortcuts in  Chromium Based Browser - but mainly made for ARC 

# AKA Chrome Extension Generator

A command-line tool for generating a basic Chrome extension based on user input. This tool creates a Chrome extension with a customizable URL, and optionally includes favicons. It also generates necessary files and directories for the extension.

## Features

- Generate a Chrome extension with a specified URL.
- Optionally include favicons.
- Creates a README file with icon requirements if favicons are included.
- Automatically names the extension based on the URL (excluding `https://` and `.com`).

## Prerequisites

- macOS with Xcode installed.

## Installation

Open the Project in Xcode

Open ChromeExtensionGenerator.xcodeproj in Xcode.
Build the Project

In Xcode, select Product > Build (or press Cmd + B).
Locate the Executable

After building, the executable will be located in ~/Library/Developer/Xcode/DerivedData/ChromeExtensionGenerator-<some_id>/Build/Products/Debug/ChromeExtensionGenerator.
Usage
Run the Executable

Open Terminal and navigate to the directory containing the executable. Run it with the following command:

bash
Copy code
./ChromeExtensionGenerator
Follow the Prompts

Include Favicons?: Enter Y to include favicons or N to exclude them.
Enter the URL: Provide the URL you want the Chrome extension to open.
Enter the Directory: Specify the directory where the Chrome extension files should be saved.
Directory Structure

The generated extension will be saved in the specified directory.
If favicons are included, an icons folder will be created with a README.txt file containing icon requirements.
Example
To generate an extension that opens https://www.example.com with favicons:

bash
Copy code
./ChromeExtensionGenerator
When prompted:

Enter Y for favicons.
Enter https://www.example.com as the URL.
Enter the desired directory path.
If favicons are not included:

Enter N when prompted about favicons.
Troubleshooting
Could not load icon 'icon.png' specified in 'browser_action': Ensure the icon.png file exists in the expected location or check the manifest file for correctness.
Could not load manifest: Verify that the manifest.json file is correctly formatted and exists in the specified directory.
Contributing
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

For more information or questions, please open an issue on the GitHub repository.

markdown
Copy code

### Key Sections in the README:

1. **Project Description**: Provides an overview of what the project does.
2. **Features**: Lists the key features of the tool.
3. **Prerequisites**: Details what you need before using the tool (e.g., macOS and Xcode).
4. **Installation**: Instructions on how to clone, build, and locate the executable.
5. **Usage**: Step-by-step guide on how to run the tool and what to expect.
6. **Example**: Provides an example usage scenario.
7. **Troubleshooting**: Common issues and their resolutions.
8. **Contributing**: How others can contribute to the project.
9. **License**: Information on the licensing of the project.

Feel free to adjust the template based on any additional information specific to your project.
