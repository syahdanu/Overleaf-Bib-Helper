# Overleaf-Bib-Helper

A UserScript to enhance Overleaf by integrating article search and BibTeX retrieval from DBLP and Google Scholar directly within the Overleaf editor.

- **GitHub Repository**: [https://github.com/Arvid-pku/Overleaf-Bib-Helper](https://github.com/Arvid-pku/Overleaf-Bib-Helper)
- **Greasy Fork Page**: [https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper](https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper)

## Features
- Search for academic articles from DBLP or Google Scholar within Overleaf.
- Retrieve and copy BibTeX entries with a single click.
- Configurable result counts (5, 10, 20, or 50 results).
- Scrollable results list for easy browsing.
- Keyboard shortcuts: Enter to search, Esc to close the popup.
- Supports multiple Google Scholar mirrors for accessibility.

## Installation

### Step 1: Install Tampermonkey
Tampermonkey is a browser extension required to run UserScripts like Overleaf-Bib-Helper. Follow these steps:

1. **Download Tampermonkey**:
   - **Chrome**: Install from the [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo).
   - **Firefox**: Install from [Mozilla Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/).
   - **Edge**: Install from the [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmleipfamncoeapigifbpdccjedebe).
   - **Safari**: Install from the [App Store](https://apps.apple.com/us/app/tampermonkey/id1482490089) (requires macOS).

2. **Enable Tampermonkey**:
   - After installation, click the Tampermonkey icon in your browser’s toolbar and ensure it’s enabled.

### Step 2: Install Overleaf-Bib-Helper
You can install the script in one of two ways:

#### Option 1: Install from Greasy Fork (Recommended)
1. Visit the [Greasy Fork page](https://greasyfork.org/zh-CN/scripts/532304-overleaf-bib-helper).
2. Click the **"Install this script"** button.
3. Tampermonkey will open a confirmation window. Click **"Install"** to add the script.
4. The script will automatically activate on Overleaf project pages (`https://www.overleaf.com/project/*`).

#### Option 2: Install from GitHub
1. Go to the [GitHub repository](https://github.com/Arvid-pku/Overleaf-Bib-Helper).
2. Open the `Overleaf-Bib-Helper.js` file in the repository.
3. Copy the entire script content.
4. In your browser, click the Tampermonkey icon > **"Create a new script"**.
5. Paste the copied code into the editor, replacing the default template.
6. Click **File > Save** in the Tampermonkey editor.
7. The script will be active on Overleaf project pages.

## Usage

### Opening the Tool
1. Open an Overleaf project in your browser (`https://www.overleaf.com/project/*`).
2. Look for a new icon in the Overleaf toolbar (a small document-like icon).
3. Click the icon to open the search popup.

### Searching for Articles
1. **Enter a Query**: Type your search term (e.g., article title, author, or keywords) into the input field.
2. **Select Source**: Choose "DBLP" or "Google Scholar" from the "Source" dropdown.
3. **Set Result Count**: Select 5, 10, 20, or 50 results from the "Results" dropdown.
4. **Start Search**:
   - Press the **Enter** key, or
   - Click the magnifying glass icon next to the input field.
5. Results will appear in a scrollable list below the input field. Scroll to browse if there are more results than fit in the popup.

### Copying BibTeX
1. Click on any result in the list (e.g., "Title@Author").
2. The BibTeX entry will be copied to your clipboard.
3. A notification will confirm success ("Copy successfully") or report an error ("Copy failed").

### Closing the Popup
- Press the **Esc** key anywhere on the page while the popup is open, or
- Click the toolbar icon again to toggle the popup closed.

## Keyboard Shortcuts
- **Enter**: Trigger a search from the input field.
- **Esc**: Close the popup from anywhere on the page.

## Notes
- **Google Scholar**: May occasionally require CAPTCHA verification. If BibTeX retrieval fails, the script will open a Google Scholar tab for manual intervention.
- **Preferences**: Your selected source and result count are saved between sessions.
- **Compatibility**: Works on Overleaf project pages only. Ensure you’re on a project URL (`https://www.overleaf.com/project/*`).

## Troubleshooting
- **Script Not Working?**
  - Ensure Tampermonkey is enabled and the script is active (check Tampermonkey dashboard).
  - Verify you’re on an Overleaf project page.
  - Reload the page or reinstall the script from Greasy Fork.
- **No Results?**
  - Check your search query for typos.
  - Try switching between DBLP and Google Scholar, as coverage differs.
- **Issues with Google Scholar?**
  - If CAPTCHA blocks access, complete it in the opened tab and retry.

## Contributing
Feel free to fork the [GitHub repository](https://github.com/Arvid-pku/Overleaf-Bib-Helper), submit issues, or create pull requests with improvements!
