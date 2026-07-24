# Portfolio Customization Guide

Open the named file in VS Code, then use `Ctrl + G` on Windows/Linux or `Cmd + G` on Mac to jump directly to a line number. Replace only the text inside square brackets (`[ ... ]`).

## 1. Home Page — `index.html`

| Line | Replace this placeholder | With |
| --- | --- | --- |
| 27 | `[INSERT YOUR CODING JOURNEY INTRODUCTION HERE]` | A short welcome introduction. |
| 41 | `[INSERT YOUR BIOGRAPHY HERE]` | Your background and story. |
| 42 | `[INSERT YOUR CODING JOURNEY GOALS HERE]` | Your goals for learning or coding. |
| 48 | `[INSERT PROJECT PREVIEW IMAGE HERE]` | A full-width Projects slide image placeholder. |
| 52 | `[INSERT SKILLS PREVIEW IMAGE HERE]` | A full-width Skills slide image placeholder. |
| 56 | `[INSERT ACHIEVEMENTS PREVIEW IMAGE HERE]` | A full-width Achievements slide image placeholder. |

### Adding your full Home-page background image

1. Create an `images` folder beside your HTML files.
2. Add your landscape image to that folder, for example `images/home-background.jpg`.
3. In `style.css`, replace `[INSERT HERO BACKGROUND IMAGE FILE NAME HERE]` on line 11 with `home-background.jpg`.

The image will fill the complete landing area. A dark overlay keeps the white text easy to read.

### Adding real images to the Home-page slides

Replace the complete image placeholder `<div>` on line 48, 52, or 56 with:

```html
<img class="slide-image" src="images/[INSERT IMAGE FILE NAME HERE]" alt="[INSERT IMAGE DESCRIPTION HERE]">
```

Use one image for Projects, one for Skills, and one for Achievements.

## 2. Projects Page — `projects.html`

| Line | Replace this placeholder | With |
| --- | --- | --- |
| 26 | `[INSERT YOUR PROJECTS PAGE HEADING HERE]` | Your Projects page heading. |
| 27 | `[INSERT YOUR PROJECTS PAGE INTRODUCTION HERE]` | A short overview of your projects. |
| 34 | `[INSERT PROJECT ONE IMAGE HERE]` | Your first project image placeholder or image. |
| 35 | `[INSERT PROJECT ONE IMAGE PATH HERE]` | Your first project image file path. |
| 39 | `[INSERT PROJECT TITLE HERE]` | Your first project name. |
| 40 | `[INSERT TECH STACK USED HERE]` | Technologies used in your first project. |
| 41 | `[INSERT PROJECT DESCRIPTION HERE]` | Your first project description. |
| 42 | `[INSERT REPOSITORY LINK HERE]` and `href="#"` | Your repository button text and repository URL. |
| 48 | `[INSERT PROJECT TWO IMAGE HERE]` | Your second project image placeholder or image. |
| 49 | `[INSERT PROJECT TWO IMAGE PATH HERE]` | Your second project image file path. |
| 53 | `[INSERT PROJECT TITLE HERE]` | Your second project name. |
| 54 | `[INSERT TECH STACK USED HERE]` | Technologies used in your second project. |
| 55 | `[INSERT PROJECT DESCRIPTION HERE]` | Your second project description. |
| 56 | `[INSERT REPOSITORY LINK HERE]` and `href="#"` | Your repository button text and repository URL. |
| 62 | `[INSERT PROJECT THREE IMAGE HERE]` | Your third project image placeholder or image. |
| 63 | `[INSERT PROJECT THREE IMAGE PATH HERE]` | Your third project image file path. |
| 67 | `[INSERT PROJECT TITLE HERE]` | Your third project name. |
| 68 | `[INSERT TECH STACK USED HERE]` | Technologies used in your third project. |
| 69 | `[INSERT PROJECT DESCRIPTION HERE]` | Your third project description. |
| 70 | `[INSERT REPOSITORY LINK HERE]` and `href="#"` | Your repository button text and repository URL. |

### Adding a real project image

1. Create an `images` folder beside your HTML files.
2. Put your image inside it, for example `images/project-one.jpg`.
3. Replace the complete `<div class="image-placeholder">...</div>` on lines 34, 48, or 62 with:

```html
<img src="images/[INSERT IMAGE FILE NAME HERE]" alt="[INSERT IMAGE DESCRIPTION HERE]">
```

4. Keep the `<figcaption>` underneath if you want the image path text to remain visible; otherwise delete that one `<figcaption>` line.

## 3. Skills Page — `skills.html`

| Line | Replace this placeholder | With |
| --- | --- | --- |
| 26 | `[INSERT YOUR SKILLS PAGE HEADING HERE]` | Your Skills page heading. |
| 27 | `[INSERT YOUR SKILLS PAGE INTRODUCTION HERE]` | A short introduction to your skills. |
| 32 | `[INSERT YOUR IMAGE GALLERY HEADING HERE]` | A title for the skills image gallery. |
| 35–38 | Gallery image placeholders | Four skills-related images, descriptions, and file paths. |
| 47–50 | `[INSERT LANGUAGE OR TOOL HERE]` | Programming languages you use. |
| 57–60 | `[INSERT WEB DEVELOPMENT SKILL HERE]` | Your web development skills. |
| 67–70 | `[INSERT ROBOTICS SKILL HERE]` | Your robotics skills. |
| 77–80 | `[INSERT GIT OR GITHUB SKILL HERE]` | Your Git and GitHub skills. |
| 87–90 | `[INSERT TOOL HERE]` | Tools, platforms, or hardware you use. |

To add more skills to any category, copy one nearby `<li>...</li>` line, paste it before the closing `</ul>`, and replace its bracketed text.

## 4. Achievements Page — `achievements.html`

| Line | Replace this placeholder | With |
| --- | --- | --- |
| 27 | `[INSERT YOUR ACHIEVEMENTS PAGE INTRODUCTION HERE]` | A short introduction to your achievements. |
| 35–37 | `[INSERT COMPETITION ACHIEVEMENT HERE]` | Competition names, placements, or results. |
| 44–46 | `[INSERT CERTIFICATION HERE]` | Certification names and dates. |
| 53–55 | `[INSERT SCHOOL AWARD HERE]` | Awards received at school. |
| 62–64 | `[INSERT FUTURE HACKATHON HERE]` | Future hackathon participation or awards. |

To add more achievements, copy a `<li>...</li>` line in the correct category and paste it before that category's closing `</ul>`.

## 5. Site-Wide Text and Style

- Navigation initials: line 13 in each HTML page.
- Footer year and name: `index.html` line 64, `projects.html` line 78, `skills.html` line 97, and `achievements.html` line 71.
- Text size and colors: edit `style.css`.
  - Home background image filename: line 11.
  - Main heading size: line 71.
  - Section heading size: line 73.
  - Regular introduction text size: line 75.
  - Navigation text size: line 49.

Line numbers are correct for the current version of the website. They will change if you add or remove lines later.
