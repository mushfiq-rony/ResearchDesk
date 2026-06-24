# ResearchDesk

A lightweight, offline-first **literature review workspace** that runs entirely in your browser. No accounts, no server, no build step, no dependencies to install — just open a single HTML file and start working.

Built for researchers and students who need to manage academic papers, annotate PDFs, synthesize ideas across sources, and draft a literature review — all in one place.

---

## Features

### Multiple Independent Workspaces (Auto-Isolated Profiles)
- Create multiple copies of the HTML file (e.g., `ResearchDesk_ProjectA.html`, `ResearchDesk_ProjectB.html`).
- The app automatically detects the file name and creates a **completely separate, isolated storage vault** for each file.
- Manage different research projects simultaneously without your data mixing.
- A visible **Profile Indicator** on the Dashboard shows which workspace you are currently using.

### Library
- Add papers manually, or **auto-fill metadata from a DOI** (powered by the free CrossRef API)
- Attach PDFs directly to each paper
- Tag, rate (1–5 stars), and organize your collection
- Set **reading priority** and **deadlines**
- Track status: *To Read → Reading → Done*
- Search and sort by title, year, rating, or priority

### PDF Reader & Annotation
- Read attached PDFs in a built-in viewer with zoom and page navigation
- **Line-by-line highlighting** — select text and it highlights following the lines
- **Box highlighting** — drag a rectangle to mark figures, equations, or regions
- Five highlight colors
- Attach **notes/comments** to any highlight
- **Eraser** tool to remove highlights quickly
- Highlights are saved per paper and persist between sessions

### Per-Paper Notes
Capture structured notes for every paper:
- Personal summary
- Key points (categorized: Insight, Method, Limitation, Finding, Theory)
- Quotes with page numbers
- Strengths
- Gaps / weaknesses
- Related-paper links

### Compiled View
See **every paper's notes aggregated in one scrollable review**. Filter across your whole library by:
- Summaries
- Strengths
- Gaps
- Key points
- Quotes

### Synthesis
- A drag-and-drop **concept map** to cluster papers into themes
- Track cross-paper **research gaps** and **agreements**
- Visualize connections between papers that share themes

### Write
- Draft your literature review **section by section**
- Live word count per section
- **Insert saved quotes** directly into your draft, auto-formatted with citation

### Citations & Export
- Generate citations in **APA, MLA, Chicago, and BibTeX**
- Export your entire review (bibliography, notes, gaps, drafts, references) as a text file
- **Back up and restore** all your data (including attached PDFs) as a single JSON file

---

## Getting Started

1. **Download** `ResearchDesk.html` from this repository.
2. **Open it** in any modern browser (Chrome, Safari, Firefox, Edge).
3. Start adding papers — that's it.

No installation, no internet connection required (except for optional DOI lookups), and all your data stays on your device.

### Use it like an app on iPad / iPhone
1. Save `ResearchDesk.html` to the **Files** app (iCloud Drive works well).
2. Open it in **Safari**.
3. Tap the **Share** button → **Add to Home Screen**.
4. Launch it from your home screen for a full-screen, app-like experience.

### Managing Multiple Projects
To work on different research projects without mixing data:
1. Make a copy of `ResearchDesk.html` and rename it (e.g., `ProjectA.html`).
2. Open the new file in your browser. 
3. The app will automatically create a fresh, isolated workspace for that file. You can verify the active profile name at the top of the Dashboard.

---

## Data & Privacy

- All data is stored **100% locally in your browser**. Nothing is uploaded to any server.
- **Smart Storage:** Metadata, notes, and settings are saved using `localStorage`, while large files like PDFs are stored using `IndexedDB` to handle hundreds of megabytes without hitting browser storage limits.
- The only outbound request is the optional DOI metadata lookup to CrossRef.
- Use the built-in **Backup** button regularly to export a JSON copy of your data (including all attached PDFs), especially before clearing browser data or switching devices.

> **Note:** Because data is tied to the specific file name and browser, clearing your browser's site data will erase your work. Always keep backups!

---

## Tech

- Single self-contained HTML file
- Vanilla JavaScript — no frameworks, no build tools
- [PDF.js](https://mozilla.github.io/pdf.js/) for PDF rendering
- [Tabler Icons](https://tabler-icons.io/) for the interface
- [CrossRef API](https://www.crossref.org/) for DOI metadata lookup

---

## Browser Support

Works in all current versions of Chrome, Safari, Firefox, and Edge. Optimized for both desktop and tablet use.

---

## License

Released under the [MIT License](LICENSE). Free to use, modify, and share.

---

## Author

Developed by **Md Mushfiqur Rahman**  
🌐 [mushfiq-rony.github.io](https://mushfiq-rony.github.io/)
