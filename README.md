# Matric Maths Academy — Grade 12 NSC

**Made by: Liyema Ndzata**

An offline-first, responsive Progressive Web App (PWA) starter for South African Grade 12 Mathematics.

## Included
- Responsive layout for phone, tablet and desktop.
- Lessons and worked examples for 12 topic areas: algebra, functions, sequences/series, finance, calculus, trigonometry, analytical geometry, statistics, probability, Euclidean geometry, vectors and mixed exam revision.
- Practice question generator with varied numerical inputs, hints, answer checks and points.
- Graph lab for quadratic, straight-line, sine and exponential curves.
- Local learner profiles and a local scoreboard.
- Links to official DBE/WCED past-paper resources.
- Service worker cache for offline use once the app has been served and installed.

## Run locally
Service workers require `localhost` or HTTPS (opening `index.html` directly from a file manager will not enable the offline cache).

1. Install Python 3 on a computer.
2. Unzip this project.
3. In the project folder, run:
   `python -m http.server 8000`
4. On the same computer, open `http://localhost:8000`.
   For phone testing on the same Wi-Fi, open `http://YOUR-COMPUTER-LAN-IP:8000` on your phone. Allow the firewall prompt if needed.
5. In the browser menu, choose **Install app** or **Add to Home screen**. Open it once while online/connected to the local server so the app assets can be cached.

For public hosting, upload the files to any static HTTPS host. Then open the HTTPS URL and install the PWA. No external JavaScript libraries are required.

## Offline and multi-user limitations
- Lessons, generated practice and graph drawing are local. After the assets are cached, these work offline.
- Learner profiles, points and topic completion are saved in browser local storage on that device/browser. This is convenient for multiple learners sharing one device, but it is **not** a secure account system.
- There is no cloud leaderboard, sign-in, cross-device synchronisation or cloud backup. Those require a backend/database, authentication and hosting.
- External past-paper links require internet. This project links to official resources rather than bundling copyrighted papers. Download the papers/memos from the official source when online if you need local copies.
- The question generator makes many variations from reusable patterns; it is not a bank of thousands of individually authored, quality-assured examination questions. Review answers and topic coverage with a qualified Mathematics teacher.
- Lessons are concise starter notes, not a complete substitute for the official CAPS curriculum, current examination guidelines, textbook or teacher.

## Suggested next steps for a production release
1. Expand and have all lesson content and questions reviewed against the latest DBE CAPS and examination guidelines.
2. Add a full offline question database, detailed step-by-step solutions, adaptive revision and more simulations.
3. Add a secure backend for learner accounts and shared leaderboards (for example, Supabase/Firebase or a custom API).
4. Add automated tests, accessibility review, Android/iOS packaging if native store distribution is required, and backup/export tools.

## Official study resources
- WCED ePortal: https://wcedeportal.westerncape.gov.za/nsc-past-exam-papers-and-memos
- DBE NSC past papers: https://www.education.gov.za/Curriculum/NationalSeniorCertificate(NSC)Examinations/NSCPastExaminationpapers.aspx
- WCED Mathematics Paper 1 (May/June 2026): https://wcedeportal.westerncape.gov.za/eresource/2026-mayjune-nsc-mathematics-p1
