# City of Redwood Falls SMS pages

Public pages for the City 10DLC text-messaging campaign.

## Files

| File | Purpose |
|---|---|
| `index.html` | Opt-in (campaign call-to-action) |
| `help.html` | HELP |
| `opt-out.html` | STOP / opt-out |
| `privacy.html` | Required SMS privacy statement |
| `terms.html` | SMS terms |
| `config.js` | Published Google Form URLs |
| `css/site.css` | Shared styles |
| `js/embed-form.js` | Loads the form into each page |

## Connect the Google Forms

1. Open **City of Redwood Falls SMS Roster** in Google Drive.
2. Open the **Form links** tab.
3. Copy the three published form URLs (not the edit URLs).
4. Paste them into `config.js`:

```js
window.CRF_SMS_FORMS = {
  optin: "https://docs.google.com/forms/d/e/..../viewform",
  help: "https://docs.google.com/forms/d/e/..../viewform",
  optout: "https://docs.google.com/forms/d/e/..../viewform"
};
```

## GitHub Pages test

1. Create a repository (for example `crf-sms`).
2. Upload this folder as the repo root.
3. Settings → Pages → Deploy from branch `main` / root.
4. Open `https://YOUR_USER.github.io/crf-sms/` (or the Pages URL GitHub shows).
5. Submit a test on Opt in, Help, and Opt out. Rows appear in the Google Sheet.

TCR / Voxtelesys campaign fields:

- Website: `https://ci.redwood-falls.mn.us/`
- Call-to-action URL: this `index.html` on Pages (move to the city site before final registration)
- Privacy policy URL: `privacy.html`
- Terms URL: `terms.html`

The privacy page must stay public, with no login.
