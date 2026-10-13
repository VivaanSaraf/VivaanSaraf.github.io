# Portfolio customization guide

Open a file in VS Code and press `Cmd + G` on Mac (`Ctrl + G` on Windows/Linux) to jump to a line. The line numbers below match this branch and will move if you edit the files.

## Home — `index.html`

| Line | What you can change |
| --- | --- |
| 27–28 | The welcome title and short sentence beside the portrait slot. |
| 35 | Replace `[ADD PORTRAIT PHOTO HERE]` with your portrait photo. |
| 46–49 | Your MakerWorks biography, second-year VEX result, photo journal, and GitHub link. |
| 56 | Projects tile photo (16:9). |
| 60 | Skills tile photo (4:3). |
| 64 | Achievements tile photo (4:3). |

The landing-page hero has a black background and a 3:4 portrait frame. Put a portrait photo in `images/`, then replace the whole placeholder `<div>` on line 35 with:

```html
<img src="images/your-portrait.jpg" alt="Portrait of Vivaan Saraf">
```

The portrait frame uses `object-fit: cover`, so the photo keeps its proportions on laptop, tablet, and phone screens.

## Projects — `projects.html`

| Line | What you can change |
| --- | --- |
| 34–44 | VEX IQ photo, story, 2nd-place result, and page link. |
| 50–60 | SO-101 photo, story, current stage, and page link. |
| 66 | Replace `[ADD OPEN DUCK MINI PHOTO HERE]` with an actual image. |
| 71–76 | Open Duck Mini V2 story, current stage, and page link. |
| 82–92 | Drone photo, story, current stage, and page link. |
| 98–108 | Arduino robot photo, story, current stage, and page link. |

To add your Open Duck photo, put the file in `images/` and replace the whole placeholder `<div>` on line 66 with:

```html
<img src="images/your-open-duck-photo.jpg" alt="Open Duck Mini V2 robot" loading="lazy">
```

The five buttons open `vex-iq.html`, `so-101.html`, `open-duck-mini.html`, `drone.html`, and `arduino-robot.html`. Each detail page links back to Projects. The VEX IQ and SO-101 detail pages also link to your shared photo journal.

## Individual project pages

| Page | What you can change |
| --- | --- |
| `vex-iq.html`, lines 31–35 and 48–52 | Beginner explanation, build story, and the team's 2nd-place result. |
| `so-101.html`, lines 31–35 and 48–52 | Beginner explanation, arm-configuration process, and current stage. |
| `open-duck-mini.html`, lines 31–35 and 48–52 | Beginner explanation, setup progress, and next walking milestone. |
| `drone.html`, lines 31–35 and 48–50 | Beginner explanation and story; fill in the bracketed build and test details on line 49. |
| `arduino-robot.html`, lines 31–35 and 48–52 | Beginner explanation and story; add the exact obstacle response and code on line 50. |

When you add a project photo, replace the placeholder `<div>` in both `projects.html` and the matching detail page with an `<img>` element using the same relative path.

## Skills — `skills.html`

| Line | What you can change |
| --- | --- |
| 27 | Introductory sentence. |
| 35–38 | Four gallery images and captions. |
| 45–48 | Python and C++ with examples of how you use or practice them. |
| 53–57 | Web development, including how you built this portfolio. |
| 62–67 | Robotics skills tied to VEX IQ, SO-101, Open Duck Mini V2, and Arduino. |
| 72–76 | Git and GitHub, including your profile link. |
| 81–87 | Tools you use, including Arduino IDE. |

Add another skill by copying one `<li>...</li>` line inside its category.

## Achievements — `achievements.html`

| Line | What you can change |
| --- | --- |
| 35–38 | VEX IQ and Coolest Projects India competition entries. Add the specific project or event details you want to show. |
| 37–40 | The 2nd-place Nationals result you confirmed and your documented team contribution. |
| 46–50 | Arduino Junior Certification story, exam result, and image. |
| 52–59 | Earlier MindChamp courses, grouped by topic. |
| 66 | Replace `[ADD VERIFIED SCHOOL AWARD HERE]` when you have an award to list. |
| 73 | Replace `[ADD HACKATHON WHEN COMPLETED]` after a future event. |

The MindChamp certificate names and years were checked against your local PDFs. The Arduino Junior certificate and 90/100 exam result came from the files you supplied. You confirmed that your team placed 2nd at Nationals in your second VEX IQ year, and you told me you took part in Coolest Projects India 2026. The Hyderabad location was checked against event reporting. No school award has been assumed.

Before sharing the site publicly, check that everyone pictured is comfortable with the photos being public. The Arduino Junior certificate image includes a QR code and certificate ID; decide whether you want those visible online.

## Images and styling

The site uses photos already in `images/`, plus a link to the Google Photos album you shared. It does not rely on the album to load the site's embedded photos. All pages share `style.css`; update colors at the top of that file and text sizes in the heading, navigation, and card rules.
