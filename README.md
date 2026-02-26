# Godot Web Project Template

A GitHub template for creating Godot games that deploy to the web.

## Getting Started

1. Click **<a href="https://github.com/acodeninja/godot-web-project/generate" target="_blank">Use this template</a>** to create a new repository from this template.
2. Go to "Settings" > "Pages" - Set "Source" to "GitHub Actions"
3. Edit the `config.yml` file to set your game's name, Godot version, and website template.

## Fix your exported Godot Game

One issue with the [godot online editor](https://editor.godotengine.org/releases/latest/) is that any games exported from the editor can fail to import.

To fix this:

1. Export a ZIP file from the Godot online engine.
2. Upload the ZIP file to the `work_in_progress/` directory.
3. Wait for your game to be fixed.

Once the game is fixed, you will find a file with the same name but suffixed with `_fixed.zip` that has the required changes needed to allow openning without errors in the godot online editor.

## Publishing your Game

1. Export a ZIP file from the Godot online engine.
2. Upload the ZIP file to the `publish/` directory.
3. Wait for your game to build and publish.

## Project Structure

### `publish/`

Upload the zip file produced by the Godot web export here. This is where your playable game lives.

### `work_in_progress/`

This is where your work in progress game lives.

Upload the zip file produced by the Godot web export here, the repo will then fix it so it can be imported into the [godot online editor](https://editor.godotengine.org/releases/latest/) without stalling.

### `docs/`

Markdown files for your game's website. Edit these to describe your game—GitHub Pages will turn them into a site automatically.

### `.github/workflows/`

Contains GitHub Actions workflows for automated builds and deployment. **Do not edit this unless you know what you are doing.**

## License

MIT
