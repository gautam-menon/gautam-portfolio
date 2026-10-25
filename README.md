# Gautam Menon — Academic Portfolio

A responsive, single-page HTML portfolio designed for PhD applications. No build tools or JavaScript packages are required.

## Preview locally

1. Extract the folder from the ZIP.
2. Open `index.html` in a browser. For best results, preview it using a local web server (for example, VS Code Live Server) so local assets behave consistently.
3. Keep the `assets` folder next to `index.html`; the research paper and CV links use relative paths.

## Included documents

- `assets/documents/Gautam-Menon-CV.pdf` — the CV provided for the portfolio.
- `assets/documents/Car-Rental-Research-Paper.pdf` — the existing research manuscript. The site labels it clearly as unpublished.

## Add your degree documents and photos

Copy your files to the matching paths below. The page places photos in context: portrait in the hero, certificates in Education, screenshots inside Projects, and workplace / campus / presentation photos beside related sections. Place files at the paths below; the placeholder disappears when a matching image is added.

| File path | Intended use |
|---|---|
| `assets/images/profile.jpg` | Professional portrait in the hero |
| `assets/images/masters-degree.jpg` | MSc certificate / graduation image |
| `assets/images/bachelors-degree.jpg` | BSc certificate / graduation image |
| `assets/degrees/masters-degree.pdf` | MSc certificate or transcript PDF (optional) |
| `assets/degrees/bachelors-degree.pdf` | BSc certificate or transcript PDF (optional) |
| `assets/projects/skin-cancer-app.jpg` | Skin cancer classification app screenshot |
| `assets/projects/on-device-ml.jpg` | WatchOS / Core ML project screenshot |
| `assets/images/office.jpg` | Workplace photo in the Professional Experience sidebar |
| `assets/images/classroom.jpg` | Campus/classroom photo below Education |
| `assets/images/presentation.jpg` | Project presentation photo below the project cards |

Image placeholders are designed to look intentional until you add your own image. For degree PDFs, you can add visible links inside the corresponding degree card in `index.html` after placing the files.

## Add your YouTube channel and featured video

Near the bottom of `index.html`, edit the `CONFIG` object:

```js
const CONFIG = {
  YOUTUBE_VIDEO_ID: "YOUR_VIDEO_ID",
  YOUTUBE_CHANNEL_URL: "https://www.youtube.com/@yourchannel",
  FEATURED_VIDEO_TITLE: "Your video title"
};
```

The video ID is the part after `v=` in a standard YouTube video URL. The channel block is styled with YouTube-inspired black/red branding and shows the supplied 4K subscriber count. The page embeds one video using YouTube's privacy-enhanced `youtube-nocookie.com` domain when a video ID is supplied; otherwise, the channel link remains visible.

## Before sharing with supervisors

- Confirm the university/programme naming and the 9.15 result format on your BSc record.
- Consider adding your thesis/project title, supervisor, project dates, data sources, methods, evaluation metrics, and repo/demo links where available.
- Keep the paper explicitly marked unpublished unless and until it is formally published.
- Replace the channel configuration and all image placeholders.
- Review which personal contact details you want public. This version uses email and LinkedIn and does not publish your phone number.

## Deploy

You can host the folder on GitHub Pages, Netlify, Firebase Hosting, or any static web host. Upload the entire folder (not only `index.html`) so local assets and PDFs remain available.


## Personal links to update

Replace the placeholder usernames and repository names in `index.html` with your real URLs: GitHub profile, skin cancer classification repo, watchOS posture repo, Chess.com profile, YouTube channel, and featured video ID. The page displays **4K subscribers** as supplied; this is not a live subscriber count. The stats strip above Education has been removed; skills appear lower on the page and are intentionally understated. Photos are placed in their related sections instead of a separate gallery.


The Contact section includes the phone number from the supplied CV (+91 99305 93727), email, LinkedIn, GitHub, YouTube, and Chess.com links. The current SI (Sportz Interactive) experience links to the official UEFA Champions League iOS app App Store listing. Replace the placeholder GitHub, YouTube, and Chess.com profile URLs before publishing.
