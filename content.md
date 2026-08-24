A `devcontainer` file can be used to configure a GitHub Codespace. By placing the file in the `.devcontainer` directory of your repository, it will automatically be used to define the environment in the Codespace as it is built.

This behaviour can be very helpful as it ensures anyone who creates a Codespace from your repository will have a consistent development environment in terms of installed tools and VS Code extensions. This can be useful for collaborative software development and creating resources for teaching.

# Mini-Example

Click on the button at the top of the page to create a Codespace from this page's repository. This Codespace has been configured with a `devcontainer` file to show a few of the possible effects. You may have to wait several seconds for each step to occur. Verify by observing the following:

1. As the Codespace is loading, watch the build progress. You should see the selected image downloading and extracting. This may take 30 seconds-1 minute.
2. A message saying "HELLO FROM THE DEVCONTAINER FILE!" should appear in the terminal a few seconds later. This demonstrates how a devcontainer can be configured to run terminal commands.
3. The file `resources/example_file.md` should automatically open in the editor.
4. The extension [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) should be installed.
    * You should see a misspelled word highlighted in the file.
    * Open the extension tab and see it is installed.
5. A Python interpreter was included in the image used. Type the command `python --version`{.bash} in the terminal - you should see the version of Python installed repeated back to you.
6. Locate and open the `.devcontainer/devcontainer.json` file. You are not expected to understand the contents, but should observe its placement in the file structure.
