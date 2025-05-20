# M3U Editor
Effortlessly manage your IPTV playlists.
[Live Demo](https://m3ueditor.netlify.app)
---
## Overview
**M3U Editor** is a web-based application that allows you to create, import, manage, edit, and export IPTV playlists in various formats (M3U, JSON, TXT). With a modern and intuitive UI, you can organize channels, manage categories, favorite streams, check channel statuses, and play streams directly in your browser.
- **Homepage:** [https://m3ueditor.netlify.app](https://m3ueditor.netlify.app)
- **Repository:** [bugsfreeweb/m3ueditor](https://github.com/bugsfreeweb/m3ueditor)
- **License:** MIT
---
## Features
- **Create, Import, and Export Playlists**  
  Start from scratch, import from files (M3U, M3U8, TXT, JSON), or import directly from a URL. Export your playlist in M3U, JSON, or TXT format.
- **Channel Management**  
  Add, edit, remove, and reorder channels. Batch edit multiple channels at once.
- **Category & Favorites**  
  Organize channels into categories, edit categories, and mark channels as favorites for quick access.
- **Channel Health Status**  
  Automatically check whether your IPTV streams are online or offline and visualize stats in a health chart.
- **Built-in Player**  
  Play streams (HLS, DASH, MP4, MKV, TS, etc.) directly in the browser using integrated video players (HLS.js, dash.js).
- **Import History & Backup**  
  Keep track of imported playlists and create backups.
- **Modern UI**  
  Responsive design, light/dark theme toggle, and drag-and-drop support for files and channel reordering.
---

## Getting Started
### Online
Simply visit the [Live Demo](https://m3ueditor.netlify.app) to start managing your playlists instantly!
### Local Development
1. **Clone the repository:**
   ```bash
   git clone https://github.com/bugsfreeweb/m3ueditor.git
   cd m3u
   ```

2. **Open `index.html` in your browser:**  
   No build step is required—the app is pure HTML, CSS, and JavaScript.
---

## Usage
- **Create a new playlist:**  
  Click "New List" and enter a playlist name.
- **Import playlists:**  
  Use "Import", "Import URL", or drag and drop files. Supported formats: `.m3u`, `.m3u8`, `.txt`, `.json`.
- **Edit channels:**  
  Add, edit, remove, reorder, or batch edit channels. Assign categories and mark as favorites.
- **Check channel status:**  
  Click "Check Status" to verify which streams are online.
- **Export playlists:**  
  Export your playlist in your preferred format.
- **Play channels:**  
  Click the play button next to any channel or favorite to open the built-in player.
---
## Supported Formats
- **M3U / M3U8** (standard IPTV format)
- **JSON** (internal format)
- **TXT** (comma-separated: `Channel Name,URL`)
---
## Technologies Used
- **JavaScript** (core app logic)
- **HTML5** (UI structure)
- **CSS** (styling, light/dark themes)
- [Feather Icons](https://feathericons.com/) (UI icons)
- [HLS.js](https://github.com/video-dev/hls.js/) (HLS playback)
- [dash.js](https://github.com/Dash-Industry-Forum/dash.js/) (DASH playback)
---
## License
This project is licensed under the [MIT License](LICENSE).
---
## Acknowledgements
- [HLS.js](https://github.com/video-dev/hls.js)
- [dash.js](https://github.com/Dash-Industry-Forum/dash.js)
- [Feather Icons](https://feathericons.com/)
---
## Author
- [bugsfreeweb](https://github.com/bugsfreeweb)
---
## Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change or improve.

---
