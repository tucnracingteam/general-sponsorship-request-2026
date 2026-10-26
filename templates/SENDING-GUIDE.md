# Publish the page and send a sponsor email

Use two pieces: GitHub Pages hosts the page and its photos; Thunderbird sends a short personal email that links to the page. Do not paste `index.html` source code into an email, and do not attach the 25.8 MB PDF by default.

The project is organized like this:

```text
index.html                         live sponsor landing page
assets/                            optimized logo and IESC photos used by the page
General Sponsorship Request/       current sponsorship PDF
templates/
  sponsor-outreach.html            copy-ready email body
  SENDING-GUIDE.md                 these instructions
```

## 1. Publish the updated page on GitHub Pages

The local folder you have is not a Git checkout, so `git push` will not work from here. Upload the files through the GitHub website, or use the team's actual Git clone if you have one.

1. Open the GitHub repository that serves the existing sponsor page. The current email points to `https://tucnracingteam.github.io/general-sponsorship-request/`, which normally maps to `tucnracingteam/general-sponsorship-request`; confirm the address and repo in **Settings → Pages**. Check the configured publishing branch and folder, then keep using that source. GitHub Pages can publish from a branch's root or a `/docs` folder.
2. Open the configured publishing folder in the repository. Replace `index.html` and upload the three optimized files to `assets/`, keeping those paths and filenames. Before committing, make sure the file list shows the `assets/` directory structure. The page uses:
   - `assets/logo-tucn-rt.png`
   - `assets/iesc-2026-team.jpg`
   - `assets/iesc-2026-workshop.jpg`
3. Keep the email files separate from the live landing page. In the repository root, choose **Add file → Create new file**, then enter `templates/sponsor-outreach.html` as the filename and copy in the contents of the local template. Repeat with `templates/SENDING-GUIDE.md`. The slash in the filename creates the `templates/` folder. Alternatively, upload those two files while preserving their paths. Keep the existing `General Sponsorship Request/Mapa Sponsorizare.pdf` in the same relative path so the offer links continue to work.
4. Commit the uploaded files. The page does not need the original high-resolution photo folder; it uses only the optimized files in `assets/`.
5. Wait for the Pages deployment to finish, then open the sponsor page in a private/incognito window and on a phone. Check that both photos load and the PDF and email buttons open the expected destinations. Do not send outreach until this published page is current.

GitHub Pages publishes the content in the selected branch/folder when changes are pushed or committed there. The site is public, so only publish files intended for sponsors.

## 2. Set up Thunderbird for formatted messages

1. In Thunderbird, open **Account Settings → your sending account → Composition & Addressing** and enable **Compose messages in HTML format**. The formatting toolbar should appear in a new message.
2. Open `templates/sponsor-outreach.html` in a browser. Copy the **rendered email** (the formatted page), not the HTML source. On Mac use **Command+A**, then **Command+C**; on Windows use **Ctrl+A**, then **Ctrl+C**.
3. In Thunderbird, choose **Write** to start a new message. Paste into the message body using the normal **Paste** command so the formatting is retained. Do not choose **Paste without formatting**.
4. Use the subject **Parteneriat pentru Australia | TUCN Racing Team**. Address one sponsor at a time, personalize the greeting with their name/company when possible, and paste the published sponsor-page URL if the button does not carry over during paste.
5. Send a test to yourself first. Open it in Gmail on desktop and phone. Check that the layout is readable, the main button opens the live page, and the offer PDF link works.
6. In the Thunderbird compose window, choose **File → Save As → Template**. For future sponsors, open the saved message from the **Templates** folder, edit the recipient and greeting, and send. The original template remains available.

## 3. Send the outreach

Send the email individually to each prospect, with a short personal opening. Keep the full dossier as an optional click-through link: the file is large, while the landing page and email body load quickly. If you later replace the dossier, update the GitHub Pages copy and verify its link before sending the next batch.

## Links and settings references

- [Thunderbird account composition settings](https://support.mozilla.org/en-US/kb/configuration-options-accounts)
- [GitHub Pages publishing source](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [GitHub Pages site visibility and publishing](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)
