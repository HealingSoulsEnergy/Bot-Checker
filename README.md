# Real or Fake?

Paste an email, a social media post or comment, a text message, a website address and its page text, a TV or online ad, a letter in the mail, or a news story or video, or add a screenshot or photo, and Real or Fake? scores how likely it is to be spam, a scam, or a bot from 0 to 100. It lists each warning sign it found and highlights the exact words in the message.

Everything runs in the browser. Pasted text is never sent anywhere. Screenshots are read on the device with Tesseract OCR (the reader downloads once from a public CDN the first time it is used, then is cached).

For websites it checks the address for lookalike brand names, letter swaps, odd endings and login bait, checks the page text for fake shop tricks, and links out to free tools (ICANN domain lookup, Google Safe Browsing, VirusTotal) that can look at the live site.

For TV and online ads it looks for fake Medicare and government benefit pitches (flex cards, giveback, $0 premium, money back in your Social Security check), miracle health claims, and call-now pressure, and it flags any phone number in a Medicare ad that isn't Medicare's real number. It then shows the real, free lines to call instead: Medicare at 1-800-633-4227 and Ohio OSHIIP at 1-800-686-1578.

For paper mail it flags letters made to look official or urgent, car warranty pitches, business filing and compliance look-alikes, prize letters that want a fee, and fine print admitting the letter is an offer and not a bill. It points to the U.S. Postal Inspection Service (1-877-876-2455, uspis.gov/report) for reporting mail fraud.

For mortgage and credit offers, in any tab, it flags letters written as if they're from your lender (mortgage protection insurance), foreclosure rescue and loan modification pitches, guaranteed approval or upfront fees, and Card Member Services, debt relief and credit repair pitches. Offers carrying the legal prescreen opt-out notice get a small credit toward looking genuine. It points to free HUD-approved housing counselors (1-800-569-4287) and the prescreen opt-out line (1-888-567-8688, optoutprescreen.com).

For news stories and videos it flags fake celebrity and Shark Tank endorsements, claims that the story is being hidden or censored, share pressure, shock headlines, missing sources, and copycat news addresses like abcnews.com.co. It does not judge whether a claim is true or take sides on any viewpoint; instead it links to Google News, Google's fact check search, and reverse image search so you can see whether real outlets report the same thing.

It also has a writing style section that shows the clues pointing toward AI writing and the clues pointing toward a person, side by side. It is a lean, never a verdict, and it never changes the spam score, because AI writing cannot be proven from text alone.

It is installable as an app on phones and computers and works offline after the first visit.

## Files

`index.html` is the whole app. `manifest.webmanifest`, `sw.js`, and the icon files make it installable.

## Putting it on GitHub Pages

Upload all the files to the root of a repository, then in the repository go to Settings, then Pages, choose Deploy from a branch, pick `main` and `/ (root)`, and save. The site appears at `https://<your-username>.github.io/<repository-name>/` within a minute or two.

When you change `index.html`, also change `CACHE` in `sw.js` (for example to `real-or-fake-v8`) so installed copies pick up the new version.

## Limits

This is a pattern checker, not a guarantee. A carefully written scam can score low, and a real store promotion can score medium. Never click a link or call a number from a message you are unsure about.

Made for Healing Souls Wellness Center.
