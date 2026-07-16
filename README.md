# NovaEdit

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-in%20active%20development-yellow.svg)
![Platforms](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey.svg)
![Built with Python](https://img.shields.io/badge/built%20with-Python-3776AB.svg)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

> A modern, lightweight, cross-platform code editor built primarily with Python.

<!-- Replace the line below with a real screenshot once one is available -->
![NovaEdit screenshot placeholder](docs/images/screenshot-placeholder.png)
*Screenshot coming soon — NovaEdit is currently in early, active development.*

> **Note:** Badge and image URLs above are placeholders. Update them once the repository, CI, and screenshots are live.

---

## Table of Contents

- [About NovaEdit](#about-novaedit)
- [Why NovaEdit Exists](#why-novaedit-exists)
- [Project Goals](#project-goals)
- [Current Status](#current-status)
- [Features](#features)
  - [Current Features (Version 0.1)](#current-features-version-01)
  - [Editor Features](#editor-features)
  - [File Explorer](#file-explorer)
  - [Themes](#themes)
  - [Settings](#settings)
  - [Built-in Browser](#built-in-browser)
  - [File Management](#file-management)
  - [Search](#search)
  - [Keyboard Shortcuts](#keyboard-shortcuts)
  - [Automatic Updates](#automatic-updates)
  - [Privacy](#privacy)
  - [Accessibility](#accessibility)
  - [Performance Goals](#performance-goals)
- [Roadmap and Planned Features](#roadmap-and-planned-features)
- [Supported Programming Languages](#supported-programming-languages)
- [Nova AI](#nova-ai)
  - [Design Philosophy](#design-philosophy)
  - [Planned Capabilities](#planned-capabilities)
  - [Project Awareness](#project-awareness)
  - [AI Privacy and Data Use](#ai-privacy-and-data-use)
- [Plugin System](#plugin-system)
  - [Plugin Philosophy](#plugin-philosophy)
- [Git Integration](#git-integration)
- [Compiler Detection](#compiler-detection)
- [Installation](#installation)
  - [System Requirements](#system-requirements)
  - [Installing on Windows](#installing-on-windows)
  - [Installing on Linux](#installing-on-linux)
  - [Installing on macOS](#installing-on-macos)
  - [Installer Options](#installer-options)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

---

## About NovaEdit

NovaEdit is a free, cross-platform code editor designed to provide a fast, clean, and beginner-friendly development experience while remaining powerful enough to grow with experienced developers.

Unlike traditional text editors that focus solely on editing files, NovaEdit is designed to become a complete **project workspace**. It combines code editing, project organization, optional AI assistance, and community-driven feature development.

The goal is not to replace every professional IDE overnight. Instead, NovaEdit aims to provide a modern alternative that starts lightweight and gradually expands through new features and community feedback.

Whether you're writing a Python script, designing a website, or managing multiple projects, NovaEdit is built to keep your workflow organized.

**[⬆ back to top](#table-of-contents)**

---

## Why NovaEdit Exists

NovaEdit began as a personal project to solve problems experienced with existing editors.

Many code editors have become increasingly large, require numerous extensions, or can be difficult for beginners to understand. Others have display or compatibility issues depending on hardware configuration.

NovaEdit aims to solve these problems by focusing on:

- Simplicity
- Performance
- Organization
- Cross-platform compatibility
- Modern user interface
- Optional advanced features instead of mandatory complexity

The philosophy behind NovaEdit is simple:

> **Start small. Grow when needed.**

Users should never feel overwhelmed by unnecessary tools. Advanced functionality should always remain optional.

**[⬆ back to top](#table-of-contents)**

---

## Project Goals

NovaEdit has several long-term goals.

| Goal | Description |
|---|---|
| **Simple** | The editor should remain easy to understand, even for someone learning programming for the first time. |
| **Fast** | The application should launch quickly, open projects quickly, and avoid unnecessary background processes whenever possible. |
| **Cross-Platform** | NovaEdit supports Windows, Linux, and macOS. All three platforms should receive the same core editing experience. |
| **Modular** | Features such as AI, plugins, additional language packs, and future developer tools are intended to be optional whenever practical. |
| **Community-Driven** | Feedback, bug reports, feature requests, and community contributions will help shape future releases. |

**[⬆ back to top](#table-of-contents)**

---

## Current Status

NovaEdit is currently under **active development**.

- The initial release focuses on providing a stable, reliable editing experience.
- Some features described throughout this document are not yet available.
- If a feature is marked as **Planned**, it is not currently implemented.
- The roadmap may change as development continues.

**[⬆ back to top](#table-of-contents)**

---

## Features

### Current Features (Version 0.1)

| Feature | Status |
|---|---|
| Modern code editor | ✅ In Progress |
| Multiple document tabs | ✅ In Progress |
| Syntax highlighting | ✅ In Progress |
| File explorer | ✅ In Progress |
| Project workspaces | ✅ In Progress |
| Theme support | ✅ In Progress |
| Custom fonts | ✅ In Progress |
| Adjustable font sizes | ✅ In Progress |
| Line numbers | ✅ In Progress |
| Search | ✅ In Progress |
| Replace | ✅ In Progress |
| Dark mode | ✅ In Progress |
| Light mode | ✅ In Progress |
| Auto-save | ✅ In Progress |
| Custom settings | ✅ In Progress |
| Cross-platform support | ✅ In Progress |
| Project configuration | ✅ In Progress |
| Workspace management | ✅ In Progress |

More features will be added in future releases.

### Editor Features

NovaEdit focuses on creating a clean editing experience.

| Feature | Status |
|---|---|
| Multiple tabs | Current |
| Line numbers | Current |
| Word wrap | Current |
| Auto indentation | Current |
| Auto save | Current |
| Find | Current |
| Replace | Current |
| Undo | Current |
| Redo | Current |
| Zoom | Current |
| Custom fonts | Current |
| Adjustable font size | Current |
| Dark mode | Current |
| Light mode | Current |
| Bracket matching | Current |
| Syntax highlighting | Current |
| Highlight current line | Current |
| Whitespace visualization | Planned |
| Minimap | Planned |
| Code folding | Planned |

### File Explorer

NovaEdit includes a built-in file explorer designed to simplify navigation. Features include:

- Create files
- Create folders
- Rename files
- Delete files
- Duplicate files
- Move files
- Drag-and-drop support *(planned)*
- Right-click context menus
- Project-wide search

The file explorer always reflects your project's actual folder structure.

### Themes

NovaEdit is designed to support extensive customization.

Planned built-in themes include:

- Nova Dark
- Nova Light
- Midnight
- Arctic
- Solar
- Classic
- High Contrast

Future versions will support downloadable community themes. Users will also be able to customize:

- Colors
- Fonts
- Cursor style
- Icon packs
- Window appearance

### Settings

NovaEdit stores editor preferences separately from project data. Examples include:

- Font size
- Font family
- Theme
- Default project location
- Startup behavior
- Autosave interval
- Search provider
- Browser preference
- AI settings
- Update preferences

Settings can be changed at any time without affecting existing projects.

### Built-in Browser

NovaEdit will eventually include an optional lightweight documentation browser, primarily to access:

- Official documentation
- Tutorials
- GitHub repositories
- Programming references
- Search engines

Users can choose their preferred search provider, including:

- DuckDuckGo
- Google
- Bing
- Custom search engine

If preferred, NovaEdit can instead open links using the user's default web browser.

### File Management

Planned capabilities include:

- Open recent projects
- Favorite projects
- Automatic project detection
- Workspace recovery
- Restore previous session
- Backup recovery
- Recent files list

Future releases may include automatic snapshots to help recover unsaved work.

### Search

NovaEdit includes project-wide search capabilities.

Planned search scopes:

- Current document
- Current project
- Open files
- Entire workspace

Advanced filters may include:

- Match case
- Whole word
- Regular expressions
- Include hidden files
- Exclude folders

### Keyboard Shortcuts

NovaEdit is designed to support familiar shortcuts used by many editors, including:

- New File
- Open File
- Save
- Save As
- Undo
- Redo
- Copy
- Paste
- Cut
- Find
- Replace
- Comment Line
- Duplicate Line
- Go to Line

Future versions will allow users to customize nearly every keyboard shortcut.

### Automatic Updates

Future releases may include an optional update system. Users will be able to:

- Check for updates manually
- Enable automatic update checks
- Skip specific versions
- View release notes before updating

Automatic updates will always remain optional.

### Privacy

NovaEdit is designed with privacy in mind.

- The editor itself does not require an internet connection to function.
- Most editing features work entirely offline.
- If optional online features are introduced in future versions, they will be clearly documented and configurable by the user.

Privacy remains a core design principle throughout the project.

### Accessibility

Planned accessibility features include:

- Adjustable font size
- Zoom controls
- High contrast themes
- Keyboard navigation
- Screen reader improvements
- Reduced motion options
- Custom color themes

Accessibility feedback is always welcome.

### Performance Goals

NovaEdit is designed with performance as a priority. Goals include:

- Fast startup
- Low memory usage
- Responsive interface
- Smooth scrolling
- Efficient file loading
- Stable performance on older hardware

Performance optimizations will continue throughout development.

**[⬆ back to top](#table-of-contents)**

---

## Roadmap and Planned Features

The table below consolidates all planned milestones into a single, de-duplicated roadmap. Planned features may change based on community feedback and development priorities.

| Version | Focus | Status |
|---|---|---|
| **0.1** | Core editor, multiple tabs, syntax highlighting, file explorer, project workspaces, themes, custom fonts, line numbers, search/replace, dark & light mode, auto-save, cross-platform support. Language support: Python, JavaScript, HTML, CSS, JSON, Markdown | 🟡 In Progress |
| **0.2** | TypeScript, YAML, and TOML support; Java and C# syntax improvements; external compiler detection; built-in terminal; Git integration; workspace improvements | ⚪ Planned |
| **0.3** | Bash, SQL, PowerShell, and Dockerfile support; Nova AI Assistant; plugin system; additional themes; workspace templates; AI project memory; documentation browser | ⚪ Planned |
| **0.4** | C, C++, Go, and Rust support | ⚪ Planned |
| **0.5** | PHP, Ruby, Perl, and Lua support | ⚪ Planned |
| **0.6** | Kotlin, Dart, and Objective-C support | ⚪ Planned |
| **0.7** | R, MATLAB, Julia, and Clojure support | ⚪ Planned |
| **0.8** | Haskell, Elixir, F#, and Lisp support | ⚪ Planned |
| **0.9** | Java and C# **compilation** support; Groovy and Visual Basic support | ⚪ Planned |
| **0.10** | **Public release** — all language support stabilized and tested in production; full cross-platform support; community plugins and themes | ⚪ Planned |
| **Future / Unversioned** | Extension marketplace, optional cloud synchronization, local AI model support, remote development, advanced debugging, collaborative editing, automatic backups, workspace sharing, language server integration, additional programming languages | ⚪ Planned |

**[⬆ back to top](#table-of-contents)**

---

## Supported Programming Languages

| Language | Introduced In | Status |
|---|---|---|
| Python | 0.1 | ✅ Available |
| JavaScript | 0.1 | ✅ Available |
| HTML | 0.1 | ✅ Available |
| CSS | 0.1 | ✅ Available |
| JSON | 0.1 | ✅ Available |
| Markdown | 0.1 | ✅ Available |
| TypeScript | 0.2 | ⚪ Planned |
| YAML | 0.2 | ⚪ Planned |
| TOML | 0.2 | ⚪ Planned |
| Bash | 0.3 | ⚪ Planned |
| SQL | 0.3 | ⚪ Planned |
| PowerShell | 0.3 | ⚪ Planned |
| Dockerfile | 0.3 | ⚪ Planned |
| C | 0.4 | ⚪ Planned |
| C++ | 0.4 | ⚪ Planned |
| Go | 0.4 | ⚪ Planned |
| Rust | 0.4 | ⚪ Planned |
| PHP | 0.5 | ⚪ Planned |
| Ruby | 0.5 | ⚪ Planned |
| Perl | 0.5 | ⚪ Planned |
| Lua | 0.5 | ⚪ Planned |
| Kotlin | 0.6 | ⚪ Planned |
| Dart | 0.6 | ⚪ Planned |
| Objective-C | 0.6 | ⚪ Planned |
| R | 0.7 | ⚪ Planned |
| MATLAB | 0.7 | ⚪ Planned |
| Julia | 0.7 | ⚪ Planned |
| Clojure | 0.7 | ⚪ Planned |
| Haskell | 0.8 | ⚪ Planned |
| Elixir | 0.8 | ⚪ Planned |
| F# | 0.8 | ⚪ Planned |
| Lisp | 0.8 | ⚪ Planned |
| Java *(compilation)* | 0.9 | ⚪ Planned |
| C# *(compilation)* | 0.9 | ⚪ Planned |
| Groovy | 0.9 | ⚪ Planned |
| Visual Basic | 0.9 | ⚪ Planned |

> Version 0.10 marks the official public release, with all language support stabilized and tested in production.

**Note on Java and C#:** syntax highlighting improvements for these languages land in 0.2, but full **compilation support** doesn't arrive until 0.9 — see [Compiler Detection](#compiler-detection) for why.

### Why isn't compiling supported immediately?

Compiling for some languages requires external software such as:

- Java Development Kit (JDK)
- .NET SDK
- C/C++ compilers
- Go toolchain

NovaEdit will **not** bundle these tools. Instead, future versions will detect whether they are installed and offer setup guidance if they are missing. This approach keeps NovaEdit lightweight while allowing developers to use their preferred compiler versions.

**[⬆ back to top](#table-of-contents)**

---

## Nova AI

**Status:** Planned (not available in Version 0.1)

Nova AI is planned as an optional assistant designed to help developers understand their projects, write cleaner code, and improve productivity.

Unlike traditional online AI assistants, Nova AI is intended to respect user choice. Users will be able to decide whether they want to use AI features at all. **The editor itself will never require AI functionality.**

### Design Philosophy

Nova AI is intended to assist developers, not replace them. It should:

- Explain code
- Help debug problems
- Suggest improvements
- Generate documentation
- Answer programming questions
- Help beginners learn programming concepts

Nova AI should never automatically rewrite an entire project without user approval.

### Planned Capabilities

Future versions may include:

- Explain selected code
- Generate comments
- Generate documentation
- Suggest bug fixes
- Detect duplicate code
- Explain compiler errors
- Generate README files
- Help organize projects
- Refactor code
- Explain APIs
- Recommend learning resources

### Project Awareness

One long-term goal is for Nova AI to understand the structure of your project instead of only individual files. For example, if a project contains:

```
Website
├── index.html
├── style.css
├── script.js
└── assets/
```

Nova AI should recognize that these files belong to the same project and provide suggestions using that context.

### AI Privacy and Data Use

Nova AI is planned to be optional. If cloud-based AI services are supported in the future, users will always be informed before data is sent to an external provider.

The goal is to support both:

- Cloud AI *(optional)*
- Local AI models *(planned)*

Users should always remain in control.

**[⬆ back to top](#table-of-contents)**

---

## Plugin System

**Status:** Planned

NovaEdit is designed with extensibility in mind. The long-term goal is to support plugins that allow users to customize and expand the editor without modifying the core application.

Possible plugin categories include:

- Themes
- Language support
- Linters
- Formatters
- AI tools
- Utilities
- Productivity tools
- Build tools
- Git enhancements

Plugins will eventually be installable from within NovaEdit.

### Plugin Philosophy

The editor should remain lightweight. Users who only need a simple editor should not be forced to install additional features. Plugins allow users to build the experience that best fits their workflow.

**[⬆ back to top](#table-of-contents)**

---

## Git Integration

**Status:** Planned

NovaEdit is planned to include built-in Git integration. Future functionality may include:

- Repository detection
- Commit history
- Branch switching
- File differences
- Commit creation
- Push
- Pull
- Merge support
- GitHub integration
- GitLab support

Git support will remain optional. Users who prefer using Git from the command line may continue doing so.

**[⬆ back to top](#table-of-contents)**

---

## Compiler Detection

**Status:** Planned for Version 0.2+

NovaEdit is primarily a code editor. It is not intended to replace language-specific compilers. Instead, NovaEdit plans to detect existing compiler installations.

| Language | Detects | If Missing |
|---|---|---|
| Python | Python installation | — |
| Java | OpenJDK, Oracle JDK | Recommends official download sources |
| C# | .NET SDK | Provides installation guidance |

### Why aren't Java and C# supported immediately?

Java and C# projects require additional software outside of NovaEdit. Rather than bundling compilers directly, NovaEdit will first focus on creating a stable editing experience. Compiler support will come later once detection and configuration can be implemented reliably.

This approach helps keep Version 0.1 focused, stable, and lightweight.

**[⬆ back to top](#table-of-contents)**

---

## Installation

NovaEdit is designed to be easy to install regardless of your operating system. Every official release will include platform-specific installers that guide you through the installation process.

**Supported Operating Systems:**

- Windows 10 (64-bit) or newer
- Windows 11
- Most modern Linux distributions
- macOS (Apple Silicon and Intel) *(planned)*

> Support for additional operating systems may be added in future releases.

### System Requirements

| | Minimum | Recommended |
|---|---|---|
| **Processor** | Modern dual-core | Quad-core |
| **RAM** | 4 GB | 8 GB or more |
| **Storage** | 500 MB available | SSD |
| **Display** | 1280×720 | 1920×1080 or higher |

NovaEdit is designed to remain lightweight while scaling well on more powerful hardware.

### Installing on Windows

1. Download the latest Windows installer from the Releases page.
2. Run the installer.
3. If prompted by Windows SmartScreen, verify the publisher and continue if you trust the release.
4. Choose an installation location or use the recommended default.
5. Select any optional components you wish to install.
6. Complete the installation.
7. Launch NovaEdit from the Start Menu or Desktop shortcut.

### Installing on Linux

Linux releases are planned to be available in multiple formats when possible, including:

- AppImage
- `.deb`
- `.rpm`

Installation methods may vary depending on your distribution.

### Installing on macOS

macOS support is planned. The installer will guide you through the installation process using standard macOS application installation methods.

### Installer Options

NovaEdit uses a guided installer to make setup simple while allowing users to choose optional components. **The editor itself is always required.**

Optional components may include:

- Nova AI
- Additional themes
- Example projects
- Future language packs
- Developer tools

Example installer options:

```
[x] NovaEdit Core (Required)
[ ] Nova AI
[ ] Additional Themes
[ ] Example Projects
[ ] Future Language Packs
```

Optional components can also be installed or removed later without reinstalling the entire application.

**[⬆ back to top](#table-of-contents)**

---

## Frequently Asked Questions

**Is NovaEdit free?**
Yes. NovaEdit is planned to remain free to use.

**Is NovaEdit open source?**
Yes — the source code is hosted on GitHub under the MIT License.

**Does NovaEdit require an internet connection?**
No. Most editor features are designed to work completely offline. Some future optional features, such as AI or update checking, may use an internet connection if enabled by the user.

**Does NovaEdit collect telemetry?**
The goal is to minimize data collection. If telemetry is ever introduced, it will be optional and clearly documented.

**Can I use NovaEdit for commercial projects?**
Yes. The editor is intended to be suitable for personal, educational, and commercial software development.

**Does NovaEdit include a compiler?**
No. NovaEdit is a code editor — compilers remain separate software installed by the user.

**Will there be extensions?**
Yes. An extension system is planned for future releases.

**[⬆ back to top](#table-of-contents)**

---

## Contributing

Contributions of all sizes are welcome. You can help by:

- Reporting bugs
- Suggesting features
- Improving documentation
- Fixing issues
- Testing pre-release versions
- Reviewing pull requests
- Creating plugins
- Developing themes

Please read `CONTRIBUTING.md` before opening an issue or submitting a pull request.

**[⬆ back to top](#table-of-contents)**

---

## Credits

NovaEdit would not be possible without the many open source projects and developer communities that inspire it. Special thanks to:

- The Python community
- Qt and PySide contributors
- Open source maintainers
- GitHub
- Everyone who contributes feedback, bug reports, feature requests, documentation, testing, and code

Community contributions help improve NovaEdit for everyone.

**[⬆ back to top](#table-of-contents)**

---

## License

NovaEdit is licensed under the **MIT License**. See the [`LICENSE`](LICENSE) file for the full license text.

**[⬆ back to top](#table-of-contents)**
