# 🌌 Wayne Search Interface

A high-performance, minimalist **New Tab replacement** designed for developers. This interface blends fluid aesthetics with deep functional utility, featuring a macOS-inspired side panel and the proprietary **Wayne Protocol**.

---

## 🚀 Quick Start

To deploy this locally, simply clone the repository and open the `index.html` file. No build steps are required.

```bash
# Clone the repository
git clone [https://github.com/samwelwayne266-coder/wayne-os.git](https://github.com/samwelwayne266-coder/wayne-os.git)
```
```bash
# Navigate to the directory
cd wayne-os
```
```bash
# Open in your browser (macOS)
open index.html
```

---

**🛠️ Key Features**

*🔍 Adaptive Search*

`Dynamic Theming` The search bar glow and border color adapt in real-time based on your chosen engine or specific "Bang" commands.

`Multi-Engine Support` Quick-toggle between Google, YouTube, and DuckDuckGo.

`Bang Shortcuts` Use prefixes like !w (Wikipedia), !gh (GitHub), or !ai (ChatGPT) to redirect queries instantly.


⚡ Wayne Protocol (wayne://)

A custom internal protocol for deep GitHub integration:
``Type wayne://[repo-name] in the search bar.``
``The system live-filters your public GitHub repositories.``
``Selecting a repo triggers the Wayne OS Side Panel to fetch and render the README.md using the GitHub API and marked.js.``

🖥️ macOS Side PanelA persistent window that serves as your system command center:Idle Mode: Displays a high-precision digital clock and system status.Documentation Mode: Renders Markdown documentation fetched via the Wayne Protocol.Interactive Controls: Fully functional "Traffic Light" buttons and vertical resizing.📋 Command GuideCommandAction!w [query]Search Wikipedia!gh [query]Search GitHub Repositoriesdefine [word]Instant dictionary definition in the UI#hexVisual preview of a HEX color code[math]Real-time calculation (e.g., 25 * 4 / 2)🎨 Technical StackFrontend: HTML5, CSS3 (Custom Flexbox), Vanilla JavaScript (ES6+).Visuals: HTML5 Canvas API for the interactive particle engine.Markdown: marked.min.js for real-time documentation rendering.APIs: Integration with GitHub REST API and Google Suggest queries.⚙️ CustomizationTo link your own GitHub account to the Wayne Protocol, modify the following line in the <script> section of index.html:JavaScript// Replace with your GitHub username in the fetch URL
const response = await fetch('[https://api.github.com/users/YOUR_USERNAME_HERE/repos?per_page=100](https://api.github.com/users/YOUR_USERNAME_HERE/repos?per_page=100)');
[!IMPORTANT]This interface requires an active internet connection to fetch GitHub repository data and live search suggestions.
