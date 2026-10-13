# Portfolio customization guide

Open a file in VS Code and press `Cmd + G` on Mac (`Ctrl + G` on Windows/Linux) to jump to a line. The line numbers below match this branch and will move if you edit the files.

## Home — `index.html`

| Line | What you can change |
| --- | --- |
| 27 | The short welcome sentence under your name. |
| 41–43 | Your MakerWorks biography, current robotics work, and the link to your shared photo journal. |
| 50 | Projects tile photo (16:9). |
| 54 | Skills tile photo (4:3). |
| 58 | Achievements tile photo (4:3). |

The full landing-page background is set by `--hero-image` on line 11 of `style.css`. Replace its path if you choose another landscape photo.

## Projects — `projects.html`

| Line | What you can change |
| --- | --- |
| 34–43 | VEX IQ photo, beginner explanation, your story, and page link. |
| 49–58 | SO-101 photo, beginner explanation, your story, and page link. |
| 64 | Replace `[ADD OPEN DUCK MINI PHOTO HERE]` with an actual image. |
| 69–73 | Open Duck Mini V2 explanation, your progress, and page link. |
| 79–88 | Drone photo, components, explanation, your story, and page link. |
| 94–103 | Arduino robot photo, explanation, your story, and page link. |

To add your Open Duck photo, put the file in `images/` and replace the whole placeholder `<div>` on line 64 with:

```html
<img src="images/your-open-duck-photo.jpg" alt="Open Duck Mini V2 robot" loading="lazy">
```

The five buttons open `vex-iq.html`, `so-101.html`, `open-duck-mini.html`, `drone.html`, and `arduino-robot.html`. Each detail page links back to Projects. The VEX IQ and SO-101 detail pages also link to your shared photo journal.

## Individual project pages

| Page | What you can change |
| --- | --- |
| `vex-iq.html`, lines 31–35 and 48–51 | Beginner explanation, followed by your build and testing story. |
| `so-101.html`, lines 31–35 and 48–51 | Beginner explanation, followed by the arm-configuration process. |
| `open-duck-mini.html`, lines 31–35 and 48–51 | Beginner explanation, followed by setup progress and the next walking milestone. |
| `drone.html`, lines 31–35 and 48–49 | Beginner explanation and your story; fill in the bracketed build and test details on line 49. |
| `arduino-robot.html`, lines 31–35 and 48–51 | Beginner explanation and your build story; add the exact obstacle response and code on line 50. |

When you add a project photo, replace the placeholder `<div>` in both `projects.html` and the matching detail page with an `<img>` element using the same relative path.

## Skills — `skills.html`

| Line | What you can change |
| --- | --- |
| 27 | Introductory sentence. |
| 35–38 | Four gallery images and captions. |
| 45–49 | Programming languages. |
| 54–58 | Web development. |
| 63–69 | Robotics, including Arduino sensors and servos. |
| 74–78 | Git and GitHub. |
| 83–89 | Tools you use, including Arduino IDE. |

Add another skill by copying one `<li>...</li>` line inside its category.

## Achievements — `achievements.html`

| Line | What you can change |
| --- | --- |
| 35–38 | VEX IQ and Coolest Projects India competition entries. Add the specific project or event details you want to show. |
| 40 | Replace `[ADD VERIFIED COMPETITION RESULTS HERE]` with your exact placing or award for each event. |
| 47 | Arduino Junior Certification title, date, and exam score. |
| 48–52 | MindChamp course certificates, grouped by topic. |
| 55 | Arduino Junior certificate image. |
| 63 | Replace `[ADD VERIFIED SCHOOL AWARD HERE]` when you have an award to list. |
| 70 | Replace `[ADD HACKATHON WHEN COMPLETED]` after a future event. |

The MindChamp certificate names and years were checked against your local PDFs. The Arduino Junior certificate and 90/100 exam result came from the files you supplied. Your VEX IQ participation certificate appears in a local photo, and you told me you took part in Coolest Projects India 2026. The Hyderabad location was checked against event reporting. No competition placement or school award has been assumed.

## Images and styling

The site uses photos already in `images/`, plus a link to the Google Photos album you shared. It does not rely on the album to load the site's embedded photos. All pages share `style.css`; update colors at the top of that file and text sizes in the heading, navigation, and card rules.
