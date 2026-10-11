# EduKonic 🚀

**Interactive classroom learning through real-world choices.**

EduKonic is a hackathon prototype from **CreatoEdu**, designed to help Pre-K–5 teachers guide collaborative, scenario-based activities and reflect on how students communicate, participate, and solve problems. The emphasis is on supporting different participation styles rather than labeling children.

## Try the live demo

After enabling GitHub Pages, replace the address below with your published URL:

**[Launch EduKonic](https://YOUR-USERNAME.github.io/EduKonic/)**

> Replace `YOUR-USERNAME` with your GitHub username. This placeholder is **not yet a live link**.

## Technology

- HTML5 for the web page structure
- CSS3 for layouts, animations, and responsive styling
- JavaScript with React 18 for app components and interactions
- HTM for JSX-like component templates without a build step
- Browser `localStorage` for saving teacher observations **on the same browser/device**

This project is a **static website**. There is no server, database, signup system, or build command. An internet connection is needed to load React, HTM, and Google Fonts from their external CDNs.

## How to run

### Live on GitHub Pages

1. Visit the [published demo](https://YOUR-USERNAME.github.io/EduKonic/) after substituting the actual username.
2. Choose **Teacher Login** or **Student Login**. These are demo-mode entry buttons; no username/password authentication is implemented.
3. Follow the steps below.

### Run locally

1. Download or clone this repository.
2. Open `index.html` in an up-to-date browser while connected to the internet.
3. If your browser restricts local-file access, serve the folder with Python:

   ```bash
   python -m http.server 8000
   ```

4. Open `http://localhost:8000`.

## Demo walkthrough

### Teacher view

1. Click **Teacher Login**.
2. From **Room 5: Sunshine Class**, click **Start Activity**.
3. Read the scenario aloud and select **Send the choice prompt to students**.
4. To simulate responses on one device, either switch to Student view and select fictional student profiles or use the teacher's **Demo tools**.
5. Watch the participation counts for **I'll Help** and **I'll Observe**. Students who don't volunteer aren't forced into a role.
6. If students volunteer, select **Pick a Random Helper**. The selected student can accept or decline. Guide the role-play and class reflection.
7. If nobody volunteers, choose **Decision Mode** to explore the question without putting anyone on the spot.
8. Use the observation form to record what you notice and review **Classroom Insights**.
9. Open **30-Day Program** for the planned program outline. **Day 1** is the interactive prototype; later days are lesson-plan previews.

### Student view

1. Select **Student Login**.
2. Choose one of the six fictional student profiles (or type a demo name).
3. Tap **Join Mission**.
4. Once the teacher starts the activity, select **I'll Help** or **I'll Observe**.
5. If selected to act, choose whether to accept the role. During reflection, answer the scenario question.
6. In the prototype, use the Teacher/Student toggle to switch views on **the same device**. Opening this page on two different devices will **not** share live classroom state.

## Features available in this prototype

- Teacher and student demo views
- A fictional class of six students
- Classroom scenario prompts and role-play
- Optional volunteering and random helper selection
- Decision Mode as an alternative to role-play
- Anonymous-style class answer summary in the demonstration
- Observation checklists and notes
- Sample-data classroom insight charts, combined with observations saved locally
- Outline of a 30-day classroom program
- Responsive, space-themed design

## Prototype limitations and privacy

- **No real-time multi-device synchronization.** Teacher and student state is held in memory in one browser session.
- **No authentication or real student accounts.** The profiles are fictional demo identities.
- **No hosted data storage.** Teacher observation entries are stored in browser `localStorage`. They remain in that browser until cleared and are not automatically shared across devices.
- **Insights include built-in sample data.** They should not be interpreted as genuine research findings or performance measures.
- **Only Day 1 is interactive.** Other days present the planned curriculum.
- **Not a diagnostic tool.** It does not assess, label, or rank children's personalities, abilities, or mental health.
- **Do not enter identifiable information about real children.** This is a hackathon prototype, not a production-ready school data system.

## How to publish using GitHub Pages

1. Sign in at [GitHub](https://github.com/) and choose **New repository**.
2. Name it `EduKonic` and make the repository **Public**.
3. Upload `index.html`, `README.md`, and `.nojekyll` to the **root** of the repository. Commit the files.
4. Go to **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Set **Branch: main** and **Folder: / (root)**. Click **Save**.
7. After GitHub finishes publishing, the demo should be at:

   `https://YOUR-USERNAME.github.io/EduKonic/`

8. Open the URL on a phone and laptop to check that the page loads and the buttons work.
9. Replace the placeholder link near the top of this README with the actual URL and commit the update.

> Repository naming and capitalization must match the URL. If the project repository is named differently, substitute its exact name.

## Add EduKonic to your CreatoEdu WordPress site

In the WordPress editor, add a **Buttons** block, label it **Try EduKonic**, and paste the GitHub Pages URL into the button's link setting. Alternatively, add a text link using the same URL. You may set it to open in a new tab so visitors can return to CreatoEdu easily.

## Project structure

```text
EduKonic/
├── index.html     # Entire working browser prototype
├── README.md      # Project, demo, and deployment instructions
└── .nojekyll      # Direct static-file deployment on GitHub Pages
```

## Next steps after the hackathon

A multi-device version would require shared state on a backend (for example, a database and real-time event service), appropriate authentication, consent and student-data safeguards, and educator testing before use with real children.

**Created for a hackathon by CreatoEdu.**
