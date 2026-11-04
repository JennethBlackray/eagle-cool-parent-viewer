# eagle-cool-parent-viewer

An inspector plugin for [Eagle](https://eagle.cool). It shows every artwork that has the same `parent:XXXX` tag as the selected image and can open the whole set in a separate viewer window.

> **This plugin is designed to work with [booru-to-eagle-cool-saver](https://github.com/JennethBlackray/booru-to-eagle-cool-saver).**
> That extension saves artworks from booru sites into Eagle and gives related images a shared `parent:<id>` tag. Parent Viewer groups images by that tag.
> It also works without the extension, but then you have to add the `parent:...` tags yourself.

## Installation

1. Download this repository (**Releases**) and unpack it to any folder.
2. In Eagle, click the **Plugin** button on the toolbar and choose **Developer Options**.
3. Click **Import Local Project** and select the unpacked folder (the one that contains `manifest.json`).
4. Select an image with a `parent:...` tag in your library. A **Parent Viewer** section with all artworks from that set appears in the right-hand panel (the inspector).

### Inspector panel

| Action | Result |
|---|---|
| Click a card | Open that artwork in Eagle |
| Middle-click a card | Open the artwork in a new window |
| Click the `parent:...` badge | Copy the tag to the clipboard |
| **👁 Watch parent** | Open the whole set in the viewer window |
| **🗑 Delete Set** | Move the whole set to the Eagle Trash |

## Viewer window controls

Open the viewer with the **👁 Watch parent** button.

### Keyboard

| Keys | Action |
|---|---|
| `→` `↓` `PageDown` `D` | Next artwork |
| `←` `↑` `PageUp` `A` | Previous artwork |
| `Home` / `End` | First / last artwork |
| `Space` | Start or stop the slideshow (3 seconds per image) |
| `+` / `-` | Zoom in / out |
| `0` | Switch between fit to window and 100% |
| `T` | Show or hide the thumbnail strip |
| `F` / `F11` | Fullscreen |
| `Esc` | Leave fullscreen; if not in fullscreen, close the window |

### Mouse

| Action | Result |
|---|---|
| Wheel over the image | Flip through artworks |
| `Ctrl` + wheel | Zoom toward the cursor |
| Double-click | Switch between fit to window and 100% |
| Drag (when zoomed in) | Move the image |
| Wheel over the thumbnail strip | Scroll the strip |
| Click a thumbnail | Go to that artwork |
| `‹` `›` arrows on the sides | Previous / next artwork |

### Toolbar buttons

- **⟳ Selected** — load the set of the image currently selected in Eagle.
- **▶ Slideshow** — start or stop the slideshow.
- **Fit** — switch between fit to window and 100%.
- **▤ Thumbs** — show or hide the thumbnail strip (the setting is remembered).
- **⛶** — fullscreen.

The slideshow stops as soon as you flip through artworks yourself.

