# Portfolio customization guide

Open a file in VS Code and press `Cmd + G` on Mac (`Ctrl + G` on Windows/Linux) to jump to a line. The line numbers below match this branch and will move if you edit the files.

## Home — `index.html`

| Line | What you can change |
| --- | --- |
| 27 | The short welcome sentence under your name. |
| 41–43 | Your biography, current robotics work, and the link to your shared photo journal. |
| 50 | Projects tile photo. |
| 54 | Skills tile photo. |
| 58 | Achievements tile photo. |

The full landing-page background is set by `--hero-image` on line 11 of `style.css`. Replace its path if you choose another landscape photo.

## Projects — `projects.html`

| Line | What you can change |
| --- | --- |
| 34–42 | VEX IQ photo, summary, and photo-journal button. |
| 48–56 | SO-101 photo, summary, and photo-journal button. |
| 62 | Replace `[ADD OPEN DUCK MINI PHOTO HERE]` with an actual image. |
| 67–70 | Open Duck Mini V2 details and photo-journal button. |

To add your Open Duck photo, put the file in `images/` and replace the whole placeholder `<div>` on line 62 with:

```html
<img src="images/your-open-duck-photo.jpg" alt="Open Duck Mini V2 robot" loading="lazy">
```

The three buttons currently open your shared Google Photos album. When you have a separate repository or project gallery, replace the relevant button's `href` with its exact URL and update its text.

## Skills — `skills.html`

| Line | What you can change |
| --- | --- |
| 27 | Introductory sentence. |
| 35–38 | Four gallery images and captions. |
| 45–49 | Programming languages. |
| 54–58 | Web development. |
| 63–68 | Robotics. |
| 73–77 | Git and GitHub. |
| 82–87 | Tools you use. |

Add another skill by copying one `<li>...</li>` line inside its category.

## Achievements — `achievements.html`

| Line | What you can change |
| --- | --- |
| 35–38 | VEX IQ and Coolest Projects India competition entries. Add the specific project or event details you want to show. |
| 40 | Replace `[ADD VERIFIED COMPETITION RESULTS HERE]` with your exact placing or award for each event. |
| 47–51 | MindChamp course certificates, grouped by topic. |
| 58 | Replace `[ADD VERIFIED SCHOOL AWARD HERE]` when you have an award to list. |
| 65 | Replace `[ADD HACKATHON WHEN COMPLETED]` after a future event. |

The certificate names and years were checked against your local certificate PDFs. Your VEX IQ participation certificate appears in a local photo, and you told me you took part in Coolest Projects India 2026. The Hyderabad location was checked against event reporting. No competition placement or school award has been assumed.

## Images and styling

The site uses photos already in `images/`, plus a link to the Google Photos album you shared. It does not rely on the album to load the site's embedded photos. All pages share `style.css`; update colors at the top of that file and text sizes in the heading, navigation, and card rules.
