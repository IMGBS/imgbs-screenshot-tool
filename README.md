# IMGBS Screenshot Tool

A free, lightweight Windows desktop app for capturing screenshots, recording GIFs, and uploading directly to [IMGBS.com](https://imgbs.com) — the free image hosting platform.

Take a screenshot, get a link. That simple.

![IMGBS Screenshot Tool](https://imgbs.com/uploads/bs-desktop-tool-0cce4404.webp)

## Download

**[Download Latest Release](https://imgbs.com/download/IMGBS-Desktop-Tool.zip)** — Windows 10 and later. No installation required — extract and run.

## Features

- **Screenshot capture** — fullscreen or select a region
- **GIF recording** — select an area, record up to 10 seconds
- **Instant upload** — link copied to clipboard automatically
- **Built-in editor** — crop and add titles before uploading
- **Drag and drop** — drop any image onto the app to upload
- **Album support** — upload directly to your IMGBS albums
- **Auto-upload mode** — skip the editor, upload instantly
- **System tray** — runs quietly in the background
- **Start with Windows** — optional auto-start on boot
- **Sound notification** — audio feedback on successful upload
- **Dark themed UI** — easy on the eyes

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `PrtSc` | Take fullscreen screenshot |
| `Ctrl+Shift+S` | Select region screenshot |
| `Space` | Stop GIF recording |
| `ESC` | Cancel recording / close editor |

## Getting Started

1. Download and extract the ZIP
2. Run **IMGBS Screenshot Tool.exe**
3. Click **Sign In** and log in with your [free IMGBS account](https://imgbs.com/register.php)
4. Take a screenshot — the link is copied to your clipboard

## How It Works

1. Press `PrtSc` for fullscreen or `Ctrl+Shift+S` to select a region
2. The editor opens — crop, add a title, pick an album (optional)
3. Click **Upload** — your image is hosted on IMGBS.com
4. The direct link is automatically copied to your clipboard
5. Paste it anywhere to share

## Requirements

- Windows 10 or later
- Internet connection
- Free IMGBS.com account

## Building From Source

Requires Python 3.10+ and the following packages:

```
pip install PyQt5 requests Pillow
```

Run the app:

```
python imgbs_screenshot.py
```

Build a standalone EXE:

```
pip install pyinstaller
pyinstaller --onefile --noconsole --name "IMGBS Screenshot Tool" --icon=icon.ico imgbs_screenshot.py
```

## Tech Stack

- **Python** — core language
- **PyQt5** — GUI framework
- **Pillow** — image processing and GIF creation
- **Requests** — API communication

## Also Available: ShareX Integration

Prefer ShareX? You can use IMGBS as a custom upload destination in ShareX. See the [ShareX Setup Guide](https://imgbs.com/sharex).

## Links

- **Website:** [imgbs.com](https://imgbs.com)
- **Download:** [imgbs.com/download](https://imgbs.com/download)
- **ShareX Guide:** [imgbs.com/sharex](https://imgbs.com/sharex)
- **API Docs:** [imgbs.com/api-docs](https://imgbs.com/api-docs)
- **Register:** [imgbs.com/register](https://imgbs.com/register.php)

## Notes

- Your API key is stored locally at `%USERPROFILE%\.imgbs-tool\` and never shared
- Windows Defender may show a SmartScreen warning on first run — this is normal for unsigned applications. Click **More info** then **Run anyway**

## License

MIT License — free to use, modify, and distribute.
