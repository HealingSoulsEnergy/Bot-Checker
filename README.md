# Spam Bot Check

Paste an email, a social media post or comment, or a text message, or add a screenshot, and Spam Bot Check scores how likely it is to be spam, a scam, or a bot from 0 to 100. It lists each warning sign it found and highlights the exact words in the message.

Everything runs in the browser. Pasted text is never sent anywhere. Screenshots are read on the device with Tesseract OCR (the reader downloads once from a public CDN the first time it is used, then is cached).

It is installable as an app on phones and computers and works offline after the first visit.

## Files

`index.html` is the whole app. `manifest.webmanifest`, `sw.js`, and the icon files make it installable.

## Putting it on GitHub Pages

Upload all the files to the root of a repository, then in the repository go to Settings, then Pages, choose Deploy from a branch, pick `main` and `/ (root)`, and save. The site appears at `https://<your-username>.github.io/<repository-name>/` within a minute or two.

When you change `index.html`, also change `CACHE` in `sw.js` (for example to `spam-bot-check-v2`) so installed copies pick up the new version.

## Limits

This is a pattern checker, not a guarantee. A carefully written scam can score low, and a real store promotion can score medium. Never click a link or call a number from a message you are unsure about.

Made for Healing Souls Wellness Center.
