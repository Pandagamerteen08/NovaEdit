Contributing to NovaEdit

Thank you for your interest in contributing to NovaEdit.

NovaEdit is built with the goal of creating a modern, lightweight, and accessible development environment for developers of all skill levels. Contributions from the community help improve the project, fix issues, add features, improve documentation, and make NovaEdit better for everyone.

Whether you are reporting a bug, suggesting a feature, improving documentation, creating themes, or contributing code, your help is appreciated.

⸻

Table of Contents

* Before Contributing
* Community and Communication
* Reporting Bugs
* Requesting Features
* Development Process
* Branch Guidelines
* Commit Guidelines
* Coding Standards
* AI-Generated Code Policy
* Pull Requests
* Plugin Contributions
* Theme Contributions
* Testing Requirements
* Documentation Contributions
* Code of Conduct
* Thank You

⸻

Before Contributing

Before making changes to NovaEdit, please make sure you understand:

* The purpose of the project
* Current development goals
* Existing features
* Planned features
* Coding standards
* Contribution requirements

Large changes should be discussed before development begins.

This helps prevent contributors from spending significant time creating features that do not match the project’s direction.

⸻

Community and Communication

The main community space for NovaEdit will be Discord.

Discord will be used for:

* Development discussions
* Community feedback
* Support
* Feature discussions
* Contribution planning
* Plugin discussions
* Theme discussions
* Testing groups

Future contribution systems may include:

* Support tickets
* Contribution requests
* Plugin submissions
* Theme submissions
* Developer channels

Official links will be available in the NovaEdit links documentation.

⸻

Reporting Bugs

Before submitting a bug report:

1. Check existing issues.
2. Confirm the issue still exists on the latest version.
3. Gather relevant information.

A useful bug report should include:

* NovaEdit version
* Operating system
* Python version (if relevant)
* Steps to reproduce the issue
* Expected behavior
* Actual behavior
* Screenshots or recordings when useful
* Error messages or logs

Example:

Issue:
Syntax highlighting stops working after opening a large file.
System:
Windows 11
NovaEdit 0.1.0
Steps:
1. Open a 20MB Python file.
2. Switch tabs.
3. Return to the file.
Expected:
Syntax highlighting remains active.
Actual:
Highlighting disappears.

Detailed reports make fixing problems much faster.

⸻

Requesting Features

Feature requests are welcome.

Before suggesting a feature, consider:

* Does it solve a real problem?
* Does it fit NovaEdit’s goals?
* Would it improve the experience for many users?

Good feature requests include:

* A description of the problem
* The proposed solution
* Possible alternatives
* Examples or screenshots when helpful

Not every requested feature will be added, but every suggestion will be considered.

⸻

Development Process

NovaEdit uses a review-based contribution process.

General workflow:

1. Discuss the idea.
2. Create a branch.
3. Make changes.
4. Test the changes.
5. Submit a pull request.
6. Review takes place.
7. Changes may be accepted, modified, or declined.

All contributions must maintain the quality and goals of NovaEdit.

⸻

Branch Guidelines

Contributors should not directly modify the main branch.

Create a separate branch for changes.

Examples:

feature/project-manager
feature/new-theme-system
bugfix/editor-crash
docs/update-installation-guide
refactor/settings-system

Recommended naming:

type/short-description

Examples:

feature/new-search-system
fix/theme-loading
docs/readme-update

⸻

Commit Guidelines

Clear commit messages make development easier.

Recommended format:

type: description

Examples:

feat: Added project templates
fix: Fixed file explorer crash
docs: Updated installation guide
refactor: Improved settings system
test: Added editor tests

Avoid unclear messages:

updated stuff
changes
fixed
new things

⸻

Coding Standards

NovaEdit uses consistent coding practices to keep the project maintainable.

Contributors should:

* Follow Python best practices
* Use clear variable names
* Write readable code
* Add comments when they improve understanding
* Avoid unnecessary complexity
* Keep functions organized
* Document important features
* Test changes before submitting

Python code should generally follow PEP 8 guidelines.

Type hints are encouraged where they improve readability.

Example:

def open_project(path: str) -> bool:
    return True

⸻

AI-Generated Code Policy

AI-assisted development is allowed.

Tools such as:

* ChatGPT
* GitHub Copilot
* Claude
* Gemini
* Other AI assistants

may be used when contributing.

However:

Contributors are responsible for all code they submit.

AI-generated code must:

* Be disclosed when used
* Be reviewed by the contributor
* Be tested
* Be understood by the contributor
* Follow NovaEdit coding standards

Submitting unreviewed AI-generated code that introduces bugs or security issues is not acceptable.

Example disclosure:

AI Assistance:
Used ChatGPT to help generate the initial structure of this function.
Reviewed and modified manually.

⸻

Pull Requests

All pull requests should include:

* Clear description of changes
* Reason for the change
* Testing performed
* Screenshots if UI changes were made
* Documentation updates if needed

Before submitting:

Checklist:

* Code works correctly
* Existing features still work
* Documentation was updated if necessary
* Code follows project standards
* Tests were completed
* AI-generated code was disclosed if used

⸻

Plugin Contributions

NovaEdit will support plugins in future releases.

Plugins will not be added directly into the main application repository unless officially approved.

Community developers may create their own plugin repositories.

Approved plugins may eventually be distributed through official NovaEdit channels.

Plugin requirements may include:

* Security review
* Documentation
* Compatibility testing
* Proper licensing
* Maintenance commitment

More information will be available when the plugin system is released.

⸻

Theme Contributions

Community-created themes will be supported in the future.

Theme creators may submit themes for consideration through the official contribution process.

Themes should:

* Follow NovaEdit design guidelines
* Include proper credits
* Avoid copyrighted material
* Be tested before submission

Approved themes may become available through official NovaEdit resources.

⸻

Testing Requirements

Contributors should test changes before submitting pull requests.

Testing may include:

* Opening the application
* Testing affected features
* Checking for errors
* Testing on supported operating systems when possible

NovaEdit aims to support:

* Windows
* Linux
* macOS

If a contributor cannot test on every platform, they should mention which platforms were tested.

⸻

Documentation Contributions

Documentation improvements are always welcome.

Examples:

* Fixing spelling errors
* Improving explanations
* Adding tutorials
* Updating outdated information
* Adding examples

Good documentation is an important part of NovaEdit.

⸻

Code of Conduct

All contributors must follow the NovaEdit Code of Conduct.

Contributors are expected to:

* Be respectful
* Communicate professionally
* Accept constructive criticism
* Avoid harassment
* Help maintain a welcoming community

The full Code of Conduct can be found in:

CODE_OF_CONDUCT.md

⸻

Final Notes

NovaEdit is built by developers, learners, and community members working together.

Every contribution matters.

Whether you submit a single typo fix, report a bug, create a theme, suggest an improvement, or contribute major code changes, your effort helps improve NovaEdit.

Thank you for helping build the future of NovaEdit.