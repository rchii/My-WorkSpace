# My Workspace

A lightweight, browser-based personal workspace dashboard for organizing links, folders, Google Drive searches, bookmarks, and frequently used web resources in one place.

## ✨ Features

- 📁 Main folders and subfolders for organizing resources
- 🔗 Add and manage website/bookmark links
- ⭐ Favorites support
- 🔎 Search saved links
- 🗃️ Google Drive search shortcut
- 📂 Google Drive folder shortcut
- 🌓 Light and dark mode
- 🕒 Date, day, time, and daily caption display
- 💾 JSON backup export
- 📥 JSON backup import and merge
- 🧭 Folder navigation with back controls
- 🕘 Recently opened links support
- 📊 Dashboard statistics
- ▶️ YouTube OTT Streaming section
- 📺 YouTube Monitoring Wall support inside the YouTube section
- 💻 Responsive layout for desktop and larger screens
- 🔒 Client-side storage using browser `localStorage`
- 🚫 No backend/database required

## 🚀 Live Demo with GitHub Pages

This project is designed to run as a static website.

### 1. Create a GitHub repository

Create a new repository, for example:

`my-workspace`

For a public GitHub Pages site, do not upload confidential work links, private IP addresses, internal server addresses, private documents, passwords, API keys, tokens, or other sensitive information.

### 2. Upload the files

Upload these files to the root of the repository:

```text
my-workspace/
├── index.html
├── README.md
├── LICENSE
├── SECURITY.md
├── .gitignore
└── .nojekyll
```

### 3. Enable GitHub Pages

Open:

`Repository → Settings → Pages`

Under **Build and deployment**:

- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/ (root)**

Save the settings.

GitHub will provide a Pages address similar to:

`https://YOUR-USERNAME.github.io/my-workspace/`

Replace `YOUR-USERNAME` and `my-workspace` with your actual GitHub username and repository name.

## 📥 Restoring your personal workspace

The GitHub version is intentionally supplied without your personal saved links. This keeps the public repository clean and prevents private bookmarks from being published.

To restore your own links on another computer/browser:

1. Open your original My Workspace dashboard.
2. Use **Export Backup**.
3. Save the JSON backup file somewhere safe.
4. Open the GitHub Pages version.
5. Use **Import Backup**.
6. Select your JSON backup.
7. Confirm the import.

The dashboard stores its working data in the browser's local storage. GitHub Pages does not automatically receive the data stored on your original computer.

## 💾 Backup recommendation

Keep at least one private copy of your JSON backup outside the public GitHub repository.

Recommended filename:

`my-workspace-backup.json`

Do **not** commit your personal backup file to a public repository if it contains private work links.

## 🔐 Privacy and security

This project is a front-end/static HTML dashboard. It does not require a server-side database for normal use.

Important:

- Browser `localStorage` is tied to the website origin.
- Your `localhost` data and GitHub Pages data are separate.
- Opening the GitHub Pages site on another device starts with a separate browser storage area.
- Private/company URLs should be kept out of the public source code.
- Do not store passwords, authentication tokens, API keys, or confidential credentials in the HTML file.
- A public GitHub repository should contain only the clean application code and non-sensitive documentation.

## 🧩 Project structure

```text
.
├── index.html       # Main My Workspace application
├── README.md        # Project documentation
├── LICENSE          # Open-source license
├── SECURITY.md      # Security and privacy guidance
├── .gitignore       # Files that should not be committed
└── .nojekyll        # Prevents unnecessary Jekyll processing on GitHub Pages
```

## 🛠️ Local testing

You can open `index.html` directly in Chrome/Edge for basic static functionality.

For a more reliable local web-server environment, run:

```powershell
python -m http.server 8080
```

Then open:

`http://localhost:8080/`

If the command is executed from the project folder, GitHub-ready `index.html` will load automatically.

## 🔄 Moving between computers

A simple workflow is:

```text
Original computer
      │
      ├── Export Backup
      │
      ▼
my-workspace-backup.json
      │
      ├── keep privately
      │
      ▼
New computer / GitHub Pages
      │
      └── Import Backup
```

## 📌 Important limitation

The current backup system is primarily designed around saved link data. Folder structure/settings that are not included in the exported JSON may need to be recreated if the application is extended later.

For a complete migration system, the backup format can be expanded to include:

- links
- main folders
- subfolders
- folder metadata
- main folder URL
- theme preference
- recently opened links
- dashboard settings

## 🧱 Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Browser Local Storage
- JSON import/export
- GitHub Pages for optional static hosting

No Node.js, npm package, database, or backend server is required for the basic dashboard.

## 🎯 Intended use

My Workspace is intended as a personal productivity dashboard for quickly reaching frequently used resources such as:

- Google Drive
- Google Sheets
- Google Docs
- YouTube tools
- Monitoring resources
- IGNOU resources
- General URLs
- Work-related shortcuts
- Daily task resources

## 📝 Customization

The dashboard can be customized by editing `index.html`.

Typical customization areas include:

- Folder names
- Icons
- Colors
- Background styling
- Captions
- Buttons
- Link categories
- YouTube monitoring configuration
- Search behavior

When modifying the application, keep private URLs and credentials outside the public repository.

## 📄 License

This project is released under the MIT License. See `LICENSE` for details.

## 🙌 Credits

Created as a custom personal workspace dashboard using standard web technologies.
