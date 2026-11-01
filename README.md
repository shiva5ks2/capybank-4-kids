# CapyBank

A pretend savings passbook for one young saver. It runs entirely in the browser on one tablet: no server, no accounts, no database.

- **Summary:** balance, next interest payment, and a chart of what she'll have in a year if she doesn't spend.
- **Passbook:** every deposit, withdrawal and interest payment, month by month.
- **Banker:** PIN-protected. Add money in or out (including backdated entries), change or cancel entries, change the interest rate, back up and restore.

Interest is 1% a month (changeable), added on the 1st, on the balance at the end of the previous month. It's worked out from the entries every time the app opens, so nothing is missed if nobody opens it on the 1st.

## Put it on GitHub Pages

1. Create a new **public** repository (for example `capybank`).
2. Choose **Add file → Upload files** and drag in everything from this folder, including the `fonts` folder. Commit.
3. Go to **Settings → Pages**. Under "Build and deployment", pick **Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. After a minute the site is live at `https://<your-username>.github.io/capybank/`.

## Set it up on her tablet

1. Open the link in **Chrome** on her tablet.
2. Fill in her name, your banker PIN and an optional opening deposit.
3. Chrome menu (⋮) → **Add to Home screen** (or **Install app**). It now opens like an app and works offline.

## Keep a backup

The data lives only in Chrome on that tablet. Clearing Chrome's data or resetting the tablet erases it.

- **Banker → Back up now** opens the share menu. Email the file to yourself.
- **Banker → Restore from backup** loads that file back, on the same tablet or a new one.
- The app reminds you if 30 days pass without a backup.

## Updating the app

Upload the changed files to the repository. If you change `index.html`, also change `capybank-v1` to `capybank-v2` in `sw.js` so the tablet picks up the new copy. Her data is not affected by updates.

## Demo Snapshots

<img width="40%" alt="02_summary_tablet" src="https://github.com/user-attachments/assets/47ecaafa-75ad-4265-8eda-53c5853a59fb" />


## Credits

Fonts: Fredoka, Atkinson Hyperlegible and Atkinson Hyperlegible Mono, under the SIL Open Font License (licences in `fonts/`).
