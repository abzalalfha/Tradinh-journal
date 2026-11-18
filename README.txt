TRADEJOURNAL — FIRST VERSION
============================

WHAT'S INCLUDED
- Offline-first trading journal for Indian options and other instruments
- Manual trade entry plus screenshot attachments
- Local IndexedDB database (no account, no cloud database)
- Dashboard, trade history, editing/deleting, strategy and mistake analysis
- Weekly review generated locally from recorded trades
- JSON export/import backup

IMPORTANT CALCULATION
Net P&L = (Exit price - Entry price) × total quantity - charges.
Choose Long (Buy first, sell to exit) or Short (Sell first, buy to exit). The app calculates the price movement in the selected direction. Quantity means total units, not lots.

WINDOWS
1. Extract this ZIP to a folder.
2. Open index.html in Microsoft Edge or Chrome.
3. For a better app-like experience, serve this folder over localhost and install from the browser's app/install menu. If Python is installed, open Command Prompt in this folder and run:
   python -m http.server 8000
   Then visit http://localhost:8000
4. Keep the folder in a location you will not delete.

IPHONE
A PWA must be served from an HTTPS website to be installable on iPhone. Upload these static files to a free HTTPS static host (for example GitHub Pages), open the HTTPS address in Safari, tap Share > Add to Home Screen. The trading data remains in IndexedDB on the iPhone; the host only serves the app files. It does not receive your journal entries.
The iPhone and Windows databases are separate. Use Export Backup on one device and Restore Backup on the other to move data.

OFFLINE
After the app has loaded once and its service worker has cached the files, the installed PWA can reopen offline. First load/install requires internet for the hosted PWA. A local Windows copy can be opened without hosting.

BACKUP
Export JSON regularly and keep a copy somewhere safe. Restoring replaces the current device's journal.

PRIVACY
No analytics, trackers, login, broker connection, or cloud database are included. Screenshots are stored in the local browser database. Clearing browser website data may erase journal data.

This is a starter build. Test calculations and backup/restore with sample trades before using it as your only record.
