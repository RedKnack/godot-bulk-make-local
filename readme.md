# Bulk Make Local

A Godot 4 editor plugin that allows making multiple scene instances local at once.

## Description

This plugin adds context menu entries to the Godot editor's scene tree when multiple nodes are selected. It provides convenient bulk operations for making scene instances local, which normally would require doing one-by-one through the editor.

## Features

- **Make Selected Local** - Makes only the selected nodes local
- **Make Selected + Children** - Makes selected nodes and all their children local recursively
- **Make ALL Local** - Makes all scene instances in the current scene local (with confirmation dialog)
- Seamless integration into the existing scene tree context menu
- Full undo/redo support
- Only appears when multiple nodes are selected

## Installation

1. Download or clone this repository
2. Copy the `addons/bulk_make_local` folder into your Godot project's `addons` directory
3. Enable the plugin in Project Settings > Plugins

## Usage

1. Select multiple nodes in the scene tree (Ctrl/Cmd + Click or Shift + Click)
2. Right-click to open the context menu
3. Choose one of the "Bulk Make Local" options at the bottom of the menu

The plugin will only add menu entries when you have multiple nodes selected.

## How It Works

The plugin hooks into Godot's editor interface and monitors for context menu popups when multiple nodes are selected. It then dynamically adds custom menu entries that perform the make local operation in bulk, properly handling the undo/redo system and scene ownership.

## Requirements

- Godot 4.0 or higher

## License

MIT License - feel free to use and modify as needed.
