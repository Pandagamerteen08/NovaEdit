NovaEdit

A modern, lightweight, cross-platform code editor built primarily with Python.

⸻

Table of Contents

* About NovaEdit
* Why NovaEdit Exists
* Project Goals
* Current Status
* Features
* Planned Features
* Supported Programming Languages
* Installation
* System Requirements
* Project Workspaces
* Customization
* Nova AI
* Plugin System
* Integrated Browser
* Compiler Detection
* Roadmap
* Frequently Asked Questions
* Contributing
* License

⸻

About NovaEdit

NovaEdit is a free, cross-platform code editor designed to provide a fast, clean, and beginner-friendly development experience while remaining powerful enough to grow with experienced developers.

Unlike traditional text editors that focus solely on editing files, NovaEdit is designed to become a complete project workspace. It combines code editing, project organization, optional AI assistance, customization, and future plugin support into a single application.

The goal is not to replace every professional IDE overnight. Instead, NovaEdit aims to provide a modern alternative that starts lightweight and gradually expands through new features and community feedback.

Whether you’re writing a Python script, designing a website, or managing multiple projects, NovaEdit is built to keep your workflow organized.

Back to Top

⸻

Why NovaEdit Exists

NovaEdit began as a personal project to solve problems experienced with existing editors.

Many code editors have become increasingly large, require numerous extensions, or can be difficult for beginners to understand. Others have display or compatibility issues depending on hardware configurations.

NovaEdit aims to solve these problems by focusing on:

* Simplicity
* Performance
* Organization
* Cross-platform compatibility
* Modern user interface
* Optional advanced features instead of mandatory complexity

The philosophy behind NovaEdit is simple:

Start small. Grow when needed.

Users should never feel overwhelmed by unnecessary tools. Advanced functionality should always remain optional.

Back to Top

⸻

Project Goals

NovaEdit has several long-term goals.

Simple

The editor should remain easy to understand, even for someone learning programming for the first time.

Fast

The application should launch quickly, open projects quickly, and avoid unnecessary background processes whenever possible.

Cross Platform

NovaEdit is designed to support:

* Windows
* Linux
* macOS

All three platforms should receive the same core editing experience.

Modular

Features such as AI, plugins, additional language packs, and future developer tools are intended to be optional whenever practical.

Community Driven

Feedback, bug reports, feature requests, and community contributions will help shape future releases.

Back to Top

⸻

Current Status

NovaEdit is currently under active development.

The initial release focuses on providing a stable, reliable editing experience.

Some planned features described throughout this document are not yet available.

If a feature is marked as Planned, it is not currently implemented.

The roadmap may change as development continues.

Back to Top

⸻

Features

Current Features (Planned for Version 0.1)

* Modern code editor
* Multiple document tabs
* Syntax highlighting
* File explorer
* Project workspaces
* Theme support
* Custom fonts
* Adjustable font sizes
* Line numbers
* Search
* Replace
* Dark mode
* Light mode
* Auto-save
* Custom settings
* Cross-platform support
* Project configuration
* Workspace management

More features will be added in future releases.

Back to Top

⸻

Planned Features

The following features are planned after the initial release.

Version 0.2

* Java syntax improvements
* C# syntax improvements
* External compiler detection
* Built-in terminal
* Git integration
* Workspace improvements

Version 0.3

* Nova AI Assistant
* Plugin system
* Additional themes
* Workspace templates
* AI project memory
* Documentation browser

Future Versions

* Extension marketplace
* Cloud synchronization (optional)
* Local AI model support
* Remote development
* Advanced debugging
* Collaborative editing
* Automatic backups
* Workspace sharing
* Language server integration
* Additional programming languages

Planned features may change based on community feedback and development priorities.

Back to Top

⸻

Supported Programming Languages

Version 0.1

Official support includes:

* Python
* JavaScript
* HTML
* CSS
* JSON
* Markdown

These languages were selected because they are text-based and do not require NovaEdit to provide compiler integration.

Planned for Version 0.2

* Java
* C#

These languages will initially receive syntax highlighting and editing support.

Why isn’t compiling supported immediately?

Compiling Java and C# requires external software such as:

* Java Development Kit (JDK)
* .NET SDK

NovaEdit will not bundle these tools.

Instead, future versions will detect whether they are installed and offer setup guidance if they are missing.

This approach keeps NovaEdit lightweight while allowing developers to use their preferred compiler versions.

Back to Top





⸻

Installation

NovaEdit is designed to be easy to install regardless of your operating system. Every official release will include platform-specific installers that guide you through the installation process.

Supported Operating Systems

* Windows 10 (64-bit) or newer
* Windows 11
* Most modern Linux distributions
* macOS (Apple Silicon and Intel, planned)

Note: Support for additional operating systems may be added in future releases.

⸻

Installing on Windows

1. Download the latest Windows installer from the Releases page.
2. Run the installer.
3. If prompted by Windows SmartScreen, verify the publisher and continue if you trust the release.
4. Choose an installation location or use the recommended default.
5. Select any optional components you wish to install.
6. Complete the installation.
7. Launch NovaEdit from the Start Menu or Desktop shortcut.

⸻

Installing on Linux

Linux releases are planned to be available in multiple formats when possible, including:

* AppImage
* .deb
* .rpm

Installation methods may vary depending on your distribution.

⸻

Installing on macOS

macOS support is planned.

The installer will guide you through the installation process using standard macOS application installation methods.

⸻

Installer

NovaEdit uses a guided installer to make setup simple while allowing users to choose optional components.

The editor itself is always required.

Optional components may include:

* Nova AI
* Additional themes
* Example projects
* Future language packs
* Developer tools

Example installer options:

☑ NovaEdit Core (Required)
☐ Nova AI
☐ Additional Themes
☐ Example Projects
☐ Future Language Packs

Optional components can also be installed or removed later without reinstalling the entire application.

Back to Top

⸻

System Requirements

Minimum

* Modern dual-core processor
* 4 GB RAM
* 500 MB available storage
* 1280×720 display

Recommended

* Quad-core processor
* 8 GB RAM or more
* SSD
* 1920×1080 or higher display

NovaEdit is designed to remain lightweight while scaling well on more powerful hardware.

Back to Top

⸻

Project Workspaces

One of NovaEdit’s primary features is its project workspace system.

Instead of opening unrelated files individually, users can organize projects into dedicated workspaces.

A workspace stores:

* Project name
* Folder location
* Open files
* Window layout
* Theme preferences
* Editor settings
* Future AI project memory

Example:

My Website
├── index.html
├── style.css
├── script.js
├── assets/
└── README.md

Each project remains independent, making it easier to manage multiple applications simultaneously.

Back to Top

⸻

File Explorer

NovaEdit includes a built-in file explorer designed to simplify navigation.

Features include:

* Create files
* Create folders
* Rename files
* Delete files
* Duplicate files
* Move files
* Drag-and-drop support (planned)
* Right-click context menus
* Project-wide search

The file explorer always reflects your project’s actual folder structure.

Back to Top

⸻

Editor Features

NovaEdit focuses on creating a clean editing experience.

Current and planned editor capabilities include:

* Multiple tabs
* Line numbers
* Word wrap
* Auto indentation
* Auto save
* Find
* Replace
* Undo
* Redo
* Zoom
* Custom fonts
* Adjustable font size
* Dark mode
* Light mode
* Bracket matching
* Syntax highlighting
* Highlight current line
* Whitespace visualization (planned)
* Minimap (planned)
* Code folding (planned)

Additional editor improvements will continue to be added throughout development.

Back to Top

⸻

Themes

NovaEdit is designed to support extensive customization.

Planned built-in themes include:

* Nova Dark
* Nova Light
* Midnight
* Arctic
* Solar
* Classic
* High Contrast

Future versions will support downloadable community themes.

Users will also be able to customize:

* Colors
* Fonts
* Cursor style
* Icon packs
* Window appearance

Back to Top

⸻

Settings

NovaEdit stores editor preferences separately from project data.

Examples include:

* Font size
* Font family
* Theme
* Default project location
* Startup behavior
* Autosave interval
* Search provider
* Browser preference
* AI settings
* Update preferences

Settings can be changed at any time without affecting existing projects.

Back to Top

⸻

Built-in Browser

NovaEdit will eventually include an optional lightweight documentation browser.

Its primary purpose is to quickly access:

* Official documentation
* Tutorials
* GitHub repositories
* Programming references
* Search engines

Users can choose their preferred search provider, including:

* DuckDuckGo
* Google
* Bing
* Custom search engine

If preferred, NovaEdit can instead open links using the user’s default web browser.

Back to Top

⸻

File Management

NovaEdit is designed to simplify working with files.

Planned capabilities include:

* Open recent projects
* Favorite projects
* Automatic project detection
* Workspace recovery
* Restore previous session
* Backup recovery
* Recent files list

Future releases may include automatic snapshots to help recover unsaved work.

Back to Top

⸻

Search

NovaEdit includes project-wide search capabilities.

Planned search options include:

* Current document
* Current project
* Open files
* Entire workspace

Advanced filters may include:

* Match case
* Whole word
* Regular expressions
* Include hidden files
* Exclude folders

Back to Top

⸻

Keyboard Shortcuts

NovaEdit is designed to support familiar shortcuts used by many editors.

Examples include:

* New File
* Open File
* Save
* Save As
* Undo
* Redo
* Copy
* Paste
* Cut
* Find
* Replace
* Comment Line
* Duplicate Line
* Go to Line

Future versions will allow users to customize nearly every keyboard shortcut.

Back to Top

⸻

Automatic Updates

Future releases may include an optional update system.

Users will be able to:

* Check for updates manually
* Enable automatic update checks
* Skip specific versions
* View release notes before updating

Automatic updates will always remain optional.

Back to Top

⸻

Privacy

NovaEdit is designed with privacy in mind.

The editor itself does not require an internet connection to function.

Most editing features work entirely offline.

If optional online features are introduced in future versions, they will be clearly documented and configurable by the user.

Privacy remains a core design principle throughout the project.

Back to Top

