Master app icon sources.

app-icon-1500-unpadded.png
  - 1500x1500 RGBA, transparent background. The color symbol, edge to edge.
  - Master for all app-icon sets (web, ios, android, desktop).

app-icon-1024-padded.png
  - 1024x1024 RGBA, transparent background.
  - Derived from app-icon-1500-unpadded.png: symbol scaled to 880px
    (~7% safe margin per side) and centered, so it doesn't clip at small
    taskbar sizes. Input for Tauri's icon generator (dashx-desktop).

To regenerate the desktop icons, run from the dashx-desktop root:

    yarn icon

That writes the platform files (icns/ico/pngs) into
dashx-desktop/src-tauri/icons/. Copy the desktop-relevant output (everything
except the android/ and ios/ subfolders) into ../desktop/ to keep this
brand-book copy in sync.
