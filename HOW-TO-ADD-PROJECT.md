# How to create a new project page

## Folder structure

```
NellaTukkiHomepage/
├── index.html
├── cv.html
├── project-template.html   ← the template (don't edit this)
├── fonts/
├── images/                 ← homepage images
└── projects/
    ├── fest/
    │   ├── index.html      ← copy of project-template.html, edited
    │   ├── images/
    │   │   ├── hero.jpg
    │   │   ├── photo-01.jpg
    │   │   ├── photo-02.jpg
    │   │   └── ...
    │   └── videos/
    │       └── performance.mp4
    ├── holobiont/
    │   ├── index.html
    │   ├── images/
    │   └── videos/
    └── metsanalaiset/
        ├── index.html
        ├── images/
        └── videos/
```

## Steps to create a new project page

1. Create a new folder inside `projects/` named after the project
   e.g. `projects/fest/`

2. Copy `project-template.html` into that folder and rename it `index.html`

3. Create `images/` and `videos/` subfolders inside it

4. Upload your photos to `images/` — name them:
   `hero.jpg` (main hero image)
   `photo-01.jpg`, `photo-02.jpg` etc. (gallery photos)

5. Upload video to `videos/` if you have one (optional)

6. Open the `index.html` and fill in:
   - Page `<title>` (line 7)
   - Project category and year (hero section)
   - Project title (hero + sidebar)
   - Premiere date, role, duration, tour dates (meta bar)
   - Performers and credits (sidebar)
   - Description text (main content)
   - Gallery image filenames
   - Video ID if using Vimeo/YouTube, or video filename if self-hosted
   - Next project link at the bottom

7. Link the project from the carousel in `index.html`:
   Find the "More about FEST" link and change `href="#"` to `href="projects/fest/"`

## Image tips
- Any photo size works — they crop automatically
- Use `class="wide"` on a gallery item for a full-width photo
- Hero image: landscape works best (at least 1400px wide)
- Gallery photos: any ratio, shown at 3:2

## Video options
- **Vimeo**: paste your Vimeo video ID into the iframe src
- **YouTube**: use `https://www.youtube.com/embed/VIDEO_ID`
- **Self-hosted**: use the `<video>` tag with src pointing to your mp4 file
- **No video**: delete the entire `project-video-section` div
