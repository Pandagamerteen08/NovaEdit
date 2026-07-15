# Project Manager Module

## Overview

The Project Manager module handles all project and workspace management functionality in NovaEdit, including project creation, file organization, and workspace handling.

## Components

### project.py
Project representation and management:
- Project metadata
- Project initialization
- Project configuration
- Project serialization/deserialization

### workspace.py
Workspace management for multiple projects:
- Workspace creation
- Project addition/removal
- Workspace persistence
- Multi-project coordination

### files.py
File and directory operations:
- File tree generation
- File operations (create, delete, move, copy)
- Directory handling
- File filtering and sorting

## Project Structure

A NovaEdit project has the following structure:

```
MyProject/
├── .nova/                      # Project metadata
│   ├── project.json           # Project configuration
│   ├── workspace.json         # Workspace settings
│   └── recent_files.json      # Recently opened files
├── src/                        # Source code
├── tests/                      # Test files
├── assets/                     # Project assets
├── docs/                       # Documentation
└── README.md                   # Project readme
```

## Usage Examples

### Creating a Project

```python
from novaedit.project_manager.project import Project

project = Project(
    name="MyProject",
    path="/path/to/project",
    language="python",
    description="My awesome project"
)
project.save()
```

### Loading a Project

```python
project = Project.load("/path/to/project")
print(f"Project: {project.name}")
print(f"Language: {project.language}")
```

### File Operations

```python
from novaedit.project_manager.files import FileManager

fm = FileManager(project)

# Create file
fm.create_file("src/main.py", "# Main file")

# Create directory
fm.create_directory("src/utils")

# List files
files = fm.get_all_files()

# Move file
fm.move_file("old/location.py", "new/location.py")

# Delete file
fm.delete_file("unwanted.py")
```

### Workspace Management

```python
from novaedit.project_manager.workspace import Workspace

workspace = Workspace(name="Development")

# Add projects
workspace.add_project(project1)
workspace.add_project(project2)

# Switch projects
workspace.set_active_project(project1)

# Save workspace
workspace.save()
```

## Project Configuration

### project.json Structure

```json
{
  "name": "MyProject",
  "version": "1.0.0",
  "description": "Project description",
  "language": "python",
  "created_at": "2024-01-15T10:30:00Z",
  "modified_at": "2024-01-15T10:30:00Z",
  "settings": {
    "indentation": 4,
    "line_endings": "LF",
    "charset": "utf-8"
  },
  "ignore_patterns": [
    "__pycache__",
    "*.pyc",
    ".venv"
  ],
  "metadata": {
    "author": "Your Name",
    "license": "MIT"
  }
}
```

## File Manager API

### FileManager Class

```python
class FileManager:
    # Initialization
    def __init__(self, project: Project)
    
    # File operations
    def create_file(path: str, content: str = "") -> File
    def delete_file(path: str) -> bool
    def move_file(source: str, destination: str) -> bool
    def copy_file(source: str, destination: str) -> bool
    def rename_file(path: str, new_name: str) -> bool
    
    # Directory operations
    def create_directory(path: str) -> Directory
    def delete_directory(path: str, recursive: bool = False) -> bool
    
    # File listing
    def get_all_files(recursive: bool = True) -> List[File]
    def get_directory_contents(path: str) -> List[File|Directory]
    def find_files(pattern: str, recursive: bool = True) -> List[File]
    
    # File info
    def get_file(path: str) -> File
    def file_exists(path: str) -> bool
    def get_file_size(path: str) -> int
    def get_file_modified_time(path: str) -> datetime
```

## Workspace API

### Workspace Class

```python
class Workspace:
    def __init__(self, name: str)
    
    # Project management
    def add_project(project: Project) -> bool
    def remove_project(project: Project) -> bool
    def get_projects() -> List[Project]
    
    # Active project
    def set_active_project(project: Project) -> bool
    def get_active_project() -> Project
    
    # Persistence
    def save() -> bool
    def load(path: str) -> Workspace
```

## Ignore Patterns

Projects support `.gitignore`-style patterns in project configuration:

```json
{
  "ignore_patterns": [
    "__pycache__/",
    "*.pyc",
    ".env",
    "node_modules/",
    "venv/",
    ".DS_Store"
  ]
}
```

## Recent Files Tracking

Workspace tracks recently opened files:

```python
# Get recent files
recent = workspace.get_recent_files(limit=10)

# Add to recent
workspace.add_to_recent(file_path)

# Clear recent
workspace.clear_recent()
```

## Project Settings

Per-project settings override global settings:

```python
# Set project-specific setting
project.set_setting("indentation", 2)

# Get setting (checks project first, then global)
indent = project.get_setting("indentation")
```

## File Watching

Optional file system watching for automatic updates:

```python
fm = FileManager(project, watch=True)

# Listen for changes
fm.on_file_changed.connect(handle_change)
fm.on_file_created.connect(handle_create)
fm.on_file_deleted.connect(handle_delete)
```

## Performance Considerations

- Large project trees are loaded incrementally
- File watching is optional for performance
- Caching of directory contents
- Lazy loading of file metadata

## Error Handling

```python
from novaedit.project_manager.files import FileError

try:
    fm.create_file("path/to/file.py")
except FileError as e:
    print(f"File operation failed: {e}")
```

## Directory Structure

```
project_manager/
├── README.md           # This file
├── project.py         # Project class
├── workspace.py       # Workspace class
└── files.py           # File operations
```

## Future Enhancements

- [ ] Project templates
- [ ] Git integration
- [ ] Project dependencies tracking
- [ ] Build configuration support
- [ ] Virtual environments management
- [ ] Project search and indexing
- [ ] Project versioning system

---

For settings integration, see `../settings/settings.py`.
For editor integration, see `../editor/editor.py`.
