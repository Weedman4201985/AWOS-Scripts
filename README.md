![AWOS Scripts Logo](logo.png)

# AWOS Scripts 🛰️

Custom userscripts for automating and enhancing the AWOS (Automated Weather Observing System) interface using the [Violentmonkey](https://violentmonkey.github.io/) extension in Firefox.

These scripts are designed to run locally within the browser extension and do not interact with the AWOS website's source code directly. They inject functionality via DOM manipulation, mutation observers, and shared utilities.

---

## 📦 Script Overview

| MAIN Scripts           | Description                                                                |
|-----------------------|-----------------------------------------------------------------------------|
| `AWOS Core 2.0 NEW.user.js`| Main automation logic. Handles DOM mutations, triggers actions, and coordinates behavior. |
| `AWOS Logger Utility 1.0.user.js`      | Logging utility. Provides a centralized `Logger` object for consistent console output. |
| `AWOS Compatibility Patch 1.0.user.js`       |Compatibility patch for AWOS Core. |

| Archived/Utility Scripts (Located in /Archived Scripts)           | Description                     |
|-----------------------|-----------------------------------------------------------------------------|
| `AWOS Mutation Observer Core 1.9.user.js`       | Main automation logic. Handles DOM mutations, triggers actions, and coordinates behavior. OLDER VERSION |
| `AWOS Mutation Observer Logging.user.js`       | Logging for Mutation Observer Core(Modular) |
| `AWOS Legacy Cleanup.user.js`       | Remove legacy scripts, config, and hidden clutter from AWOS pages. | 
| `AWOS Layout Enhancer (Full Version).user.js`       | Restore and enhance AWOS report layout with full styling.|
| `AWOS Banner Refactor.user.js`      | Reorganize AWOS banner layout using DOM manipulation and CSS injection.    |
| `WET Plugin Override + Remote Logging.user.js`       | Suppress unused WET(Web Experience Toolkit) plugins.|

| IN DEVELOPMENT Scripts            | Description                                                     |
|-----------------------|-----------------------------------------------------------------------------|
| `awos-style.js`       | Injects custom CSS to improve readability, highlight elements, or modify layout. | 
| `awos-utils.js`       | Shared helper functions used across multiple scripts (e.g., selectors, timers). |
| `awos-config.js`      | Optional configuration file for toggling features or setting thresholds.    |


---

## 🛠️ Installation Instructions

1. Install [Violentmonkey](https://violentmonkey.github.io/) in Firefox.
2. Open the Violentmonkey dashboard.
3. Click **"Create a new script"** for each file in this repository.
4. Copy-paste the contents of each script into its respective editor.
5. Save and enable each script.
6. Drag `AWOS Logger Utility 1.0.user.js` to the top of the load order to ensure `Logger` is available to other scripts.

---

## 🔁 Recommended Load Order

1. `AWOS Logger Utility 1.0`
2. `AWOS Core 2.0 NEW` 
3. `AWOS Compatibility Patch 1.0`

This ensures dependencies are available before scripts that rely on them.

---

## 🧠 Notes

- These scripts are **not hosted externally** and rely entirely on local injection via Violentmonkey.
- If the Firefox profile or extension is deleted, you can restore scripts by re-downloading them from this repository.
- All scripts are written in vanilla JavaScript and designed to be modular and maintainable.

---

## 📌 License

MIT License — feel free to use, modify, and share.

---

## 🙋‍♂️ Author

Created and maintained by **Chris**.  
If you have suggestions, feel free to open an issue or submit a pull request.


