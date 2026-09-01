# 💸 Ledger — a local-first budgeting app

A clean, private budgeting app that runs entirely in your browser. No accounts, no cloud, no server, no tracking. Your data is saved on **your** device and stays there. Perfect for running on a Mac.

Track spending, set category budgets, save toward goals, build money habits, and get a fresh tip every week — all in one page.

---

## ✨ Features

- **Spending tracker** — log expenses and income in seconds
- **Categories with budgets** — set a monthly cap per category and watch the bars fill
- **Savings goals** — set targets, log deposits, see your progress
- **Monthly habit tracker** — check off money habits each month with streak counters 🔥
- **Weekly tips** — a rotating money tip appears on your overview each week
- **6 themes** — Dawn, Midnight, Bloom, Forest, Slate, and Mono (with a custom accent color picker)
- **Auto-save** — everything persists in the browser. Close the tab, quit the browser, restart the Mac — nothing is lost
- **Backup & restore** — export your data to a file and import it anytime, or move it to another device
- **Month summary** — net cash flow, biggest category, budget performance, goals funded

Everything you and another person do stays separate, because each browser/device keeps its own private copy of the data.

---

## 🚀 How to run it (Mac)

You only need the file `index.html`. Pick whichever way is easiest.

### Option A — just double-click (simplest)
1. Download this repository (green **Code** button → **Download ZIP**), then unzip it.
2. Double-click **`index.html`**. It opens in your default browser and works immediately.
3. Bookmark it, or drag the tab to your Dock, so it's always one click away.

> Tip: keep using the **same browser** every time — your data lives in that browser's storage.

### Option B — run a tiny local server (optional)
If you'd rather open it at a web address, open the **Terminal** app, then:

```bash
cd ~/Downloads/budget-app     # or wherever you unzipped it
python3 -m http.server 8000
```

Then visit **http://localhost:8000** in your browser. (macOS already includes `python3`.)

---

## 💾 Where is my data? Is it safe?

- Your data is stored in your browser's **localStorage**, on your device only.
- It survives closing the tab, quitting the browser, and restarting your Mac.
- It is **never** sent anywhere — there's no internet connection involved after the page loads.
- The only thing that clears it is manually wiping your browser data (or clicking **Reset everything** in Settings).
- Use **Settings → Export backup** any time to save a `.json` copy you can re-import later.

Because storage is per-browser, two people on two different Macs (or even two different browsers) each get their own private budget automatically.

---

## 🎨 Themes

Go to **Settings → Theme** and pick one. Choose **Mono** to unlock a custom accent color picker and make it your own.

---

## 🛠 Tech

One self-contained `index.html` — plain HTML, CSS, and JavaScript. No build step, no dependencies, no npm install. Fonts load from Google Fonts when online, with system-font fallbacks offline.

---

## 📄 License

MIT — free to use, change, and share.
