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
| 34–42 | VEX IQ photo, summary, and link to its own page. |
| 48–56 | SO-101 photo, summary, and link to its own page. |
| 62 | Replace `[ADD OPEN DUCK MINI PHOTO HERE]` with an actual image. |
| 67–70 | Open Duck Mini V2 details and link to its own page. |
| 76–84 | Drone photo, components, summary, and page link. |
| 90–98 | Arduino robot photo, summary, and page link. |

To add your Open Duck photo, put the file in `images/` and replace the whole placeholder `<div>` on line 62 with:

```html
<img src="images/your-open-duck-photo.jpg" alt="Open Duck Mini V2 robot" loading="lazy">
```

The five buttons open `vex-iq.html`, `so-101.html`, `open-duck-mini.html`, `drone.html`, and `arduino-robot.html`. Each detail page links back to Projects. The VEX IQ and SO-101 detail pages also link to your shared photo journal.

## Individual project pages

| Page | What you can change |
| --- | --- |
| `vex-iq.html` | Main photo, build notes, and three-photo gallery. |
| `so-101.html` | Main photo, setup checklist, and three-photo gallery. |
| `open-duck-mini.html` | Photo placeholders, setup steps, and next milestone. |
| `drone.html`, lines 34–56 | Add the drone photo, exact parts and test details, and gallery photos. |
| `arduino-robot.html`, lines 34–58 | Add the robot photo, exact behaviour/code details, and gallery photos. |

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
