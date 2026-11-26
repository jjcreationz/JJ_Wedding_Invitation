# Burgundy & Champagne Gold Wedding Website

A responsive static wedding invitation site for GitHub Pages. It uses plain HTML, CSS and JavaScript — no paid hosting, build tools or framework needed.

## Included
- Burgundy / wine red / champagne gold / warm ivory theme
- Responsive desktop and mobile layout
- Wedding countdown
- Couple profiles and photo gallery
- Event schedule
- Invitation video player
- Google Maps venue link
- WhatsApp RSVP form
- Shareable invitation link
- English / Telugu / Hindi heading and navigation translations
- User-initiated background music button

## Step 1 — Edit the wedding details
Open `index.html` in a text editor (VS Code is recommended). Search for `const CONFIG = {` near the bottom and replace the sample values:
- `bride`, `groom`
- `weddingDate` (example: `2027-02-14T10:30:00+05:30`)
- `displayDate`, `city`
- `brideBio`, `groomBio`
- `venueName`, `venueAddress`, `venueDateTime`
- `mapsUrl` (paste the Google Maps share link)
- `whatsappNumber` (digits only, including country code; India example format: `91` + 10-digit mobile number)
- Event names, dates, times and places

Do not leave the sample date or WhatsApp number in the published website.

## Step 2 — Add your photos, video and music
Put your files inside `assets/` and use these exact names, or change the matching paths in CONFIG:
- `bride.jpg`
- `groom.jpg`
- `gallery-1.jpg` to `gallery-6.jpg`
- `wedding-invitation.mp4`
- `background-music.mp3`
- Optional decoration: `floral-corner.png`

Use your own images and music, or media you have permission to publish. Keep video and image files reasonably compressed so the site loads quickly on phones. Background music will only start after a visitor taps the music button because browsers restrict autoplay.

## Step 3 — Create a new GitHub repository
1. Sign in to GitHub.
2. Click the **+** button in the top-right, then **New repository**.
3. Name it something like `Our-Wedding-Invitation`.
4. Choose **Public** (GitHub Pages is available for public repositories on the free plan).
5. Select **Add a README file** if you want, then click **Create repository**.

## Step 4 — Upload the website
1. In the new repository, click **Add file → Upload files**.
2. Upload `index.html`, `README.md`, and the `assets` folder with your media files inside.
3. Scroll down and click **Commit changes**.

Important: `index.html` must be in the repository root (the first page you see), not inside another folder.

## Step 5 — Turn on GitHub Pages
1. Open the repository **Settings** tab.
2. In the left sidebar, choose **Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Set **Branch** to `main` and folder to `/(root)`.
5. Click **Save**.
6. Wait a few minutes. Refresh the Pages section; GitHub will show your published site address:
   `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`

## Step 6 — Test it
Open the published link on a phone and computer. Test:
- Countdown and displayed date
- Event details and venue Maps link
- Photo and video loading
- Music button (tap to start)
- Language selector
- Share button
- RSVP WhatsApp link

## Updating later
Edit `index.html` or upload replacement media files in GitHub. Commit the changes; GitHub Pages will publish the update automatically.

## Notes / limitations
- RSVP currently opens WhatsApp with a pre-filled message; it does not save responses to a database or spreadsheet.
- The language selector translates the navigation and selected headings. Other custom text should be translated separately if you want a fully multilingual site.
- The site is a static website; no guest login, admin dashboard or database is included.
- You can keep the repository public but avoid putting private phone numbers, personal documents or sensitive guest data in it.
