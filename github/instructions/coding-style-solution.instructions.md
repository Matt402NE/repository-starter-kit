---
applyTo: "**/*.sln"
---
# Visual Studio Solution File Coding Style

## General Guidelines
A .NET solution is described by a text file ending with the .sln extension.

- A new .NET solution should start as a blank solution.
-  A README.md file should exist in the same folder as the .sln file. The [[Template-README]] file should be used as a template to create a new README.md file when it doesn't exist.
- A CHANGELOG.md file should exist in the same folder as the .sln file. The [[Template-CHANGELOG]] file should be used as a template to create a new CHANGELOG.md file when it doesn't exist.
- A .NET solution should contain a virtual *Solution Folder* named 'Solution Items'.  The virtual folder is visible in Visual Studio.
	- The README.md and CHANGELOG.md files should be included in the virtual 'Solution Items' folder within Visual Studio.
- A .github/ folder should exist 

### COPILOT-INSTRUCTIONS
A COPILOT-INSTRUCTIONS.md file should be included in the Visual Studio solution. A copy of the Template-COPILOT-INSTRUCTIONS.md file should be placed in the .github/ folder that is within the root of the solution folder. The .github/ folder needs to be created if it doesn't already exist.

- In Visual Studio IDE, you can enable or disable these custom instructions via **Tools > Options**, searching for "custom instructions," and toggling the setting **(Preview) Enable custom instructions to be loaded from .github/copilot-instructions.md files and added to requests**.

## Naming Conventions
- Use `Proper Case` for solution name.
- The name of the solution is normally `{Full Solution Name} .NET Solution`
# References
- Context by Microsoft for [What are solutions and projects in Visual Studio?](](https://learn.microsoft.com/en-us/visualstudio/ide/solutions-and-projects-in-visual-studio?view=vs-2022))