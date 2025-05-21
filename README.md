# IPTV Playlist (M3U) editor & Channel Manager
A modern, fully client-side web application for managing, editing, importing, exporting, and playing IPTV playlists (M3U, TXT, JSON). Works offline, supports favorites, categories, drag-and-drop channel sorting, dark/light themes, health checking, and much more.

---
## Features
- **Playlists:** Create, import, export, backup, and manage multiple playlists.
- **Channels:** Add, edit, delete, reorder (drag & drop, touch and mouse), play (with HLS, MP4, DASH), open in external player.
- **Categories:** Organize channels using categories; batch-assign or edit categories.
- **Favorites:** Mark/unmark channels as favorites, quick access to all favorites.
- **Import/Export:** Import from local file (M3U, TXT, JSON) or URL (with CORS fallback), export in multiple formats.
- **Health Check:** Batch-check online/offline status of all channels (with CORS fallback and proxy support), visual health chart.
- **History & Backup:** Import history, backup/restore playlists, clear history/backups.
- **Modern UI:** Responsive for desktop and all mobile devices (landscape & portrait), accessible, keyboard navigable.
- **Theming:** Toggle between dark/light mode, with persistent theme preference.
- **Notifications:** Animated in-app notifications for actions and errors.
- **Persistence:** LocalStorage for playlists, preferences, and UI state.
- **Performance:** Lazy rendering for large channel lists, infinite scroll style loading.
---

## Quick Start
1. **Clone or Download** the repository.
2. **Open `index.html` in your browser.**
3. **No server required!** All features work offline (except URL import and health check, which require internet).
---
## Main Concepts
### State Management
A central `state` object tracks all playlists, channels, categories, favorites, history, editing state, and UI flags (like collapsed categories or health chart visibility).
### DOM Elements
All UI elements are queried once at the start and stored in the `elements` object for rapid access throughout the app. This enables fast, maintainable event binding and updates.
### Theme & Accessibility
- Toggle between dark/light themes.
- Icons automatically switch for the current theme.
- Theme is remembered across sessions.
- All dialogs/modals are keyboard and screen reader friendly.
### Playlists & Channels
- **Create** new playlists, or **import** from file/URL (supports `.m3u`, `.m3u8`, `.json`, `.txt`).
- **Export** playlists in M3U, JSON, or TXT formats (all, online only, or favorites only).
- **Backup** any playlist for safe-keeping or rollback.
- **Drag-and-drop** both via mouse and touch to reorder channels.
- **Batch edit** multiple channels at once (category, favorite flag).
### Categories & Favorites
- **Categories** can be added, renamed, deleted, and assigned per-channel or in batch.
- **Favorites** are global and persistent; mark/unmark any channel as a favorite.
### Channel Health Checking
- Batch-checks status of all channels (online/offline) using HEAD requests (with CORS fallback).
- Visual chart displays total/online/offline channels.
- Status is shown in the channel list and filterable.
### Notifications
- Toast-style notifications appear for key actions (success, error, info).
- Animations for show/hide.
---
## File Structure
- `index.html` — Main UI (responsive, mobile-first).
- `styles.css` — Modern, responsive CSS with dark/light theme support.
- `script.js` — Main application logic (see code sample above).
- (Optionally) `README.md` — You are here!
---
## Usage Tips
- **Import**: Drag-and-drop, file picker, or URL. Supported: `.m3u`, `.m3u8`, `.json`, `.txt`.
- **Export**: Choose format and channels to include (all, online, favorites).
- **Reorder**: Drag-and-drop to sort channels.
- **Health Check**: Use the "Check Status" button to update all channel statuses.
- **Theme**: Use the theme toggle button (moon/sun icon) to switch between light and dark.
- **Favorites**: Click the star to mark/unmark any channel as favorite.
- **Batch Edit**: Select multiple channels and edit category/favorite in one action.
---
## Keyboard Shortcuts
- `Tab`/`Shift+Tab`: Navigate UI elements.
- `Enter`/`Space`: Activate buttons and actions.
- `Esc`: Close modals/dialogs.
---
## Dependencies
- [Feather Icons](https://feathericons.com/) — For UI icons.
- [HLS.js](https://github.com/video-dev/hls.js) — For HLS (m3u8) stream playback.
- [Dash.js](https://github.com/Dash-Industry-Forum/dash.js) — For MPEG-DASH playback.

*(All dependencies are loaded via CDN.)*

---
## Limitations
- Health checking and stream playback from remote URLs may require CORS proxy if the resource does not support CORS.
- All data is stored in your browser only (no server, no sync).
- For large playlists (thousands of channels), performance may degrade on very old devices.
---
## License
[MIT](LICENSE)

---
## Author
- [bugsfreeweb](https://github.com/bugsfreeweb)
---
## Contribution
PRs and issues are welcome! Please open an issue or pull request for suggestions or fixes.
