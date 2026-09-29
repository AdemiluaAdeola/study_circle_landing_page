# StudyCircle

StudyCircle is a single-page landing site for a proposed Nigerian learning platform for JAMB, WAEC, and NECO candidates. It presents a pilot concept that combines bookable tutors with adaptive, syllabus-grounded practice.

## What the page includes

- **An interactive practice diagnostic** for Mathematics, Use of English, and Physics. Answer five questions to see difficulty adapt to your responses, review explanations and syllabus-topic references, and get a recap of topics to practise. The question bank is hand-written for the demo and the adaptive flow runs entirely in your browser.
- **A tutor and booking walkthrough** explaining tutor verification, escrow-held payments, booking states, and cancellation or no-show scenarios.
- **An AI and syllabus-retrieval walkthrough** showing how practice questions could be grounded in relevant syllabus passages.
- **Tutor payout and practice plan previews**, including an adjustable payout estimate and Free and Circle+ plan details.
- **Student and tutor pilot sign-up UI** with a role-specific exam or subject selector.
- Responsive layouts, keyboard-accessible interactions, reduced-motion support, and progressive enhancement for web fonts.

## Run locally

No build step, package installation, or server-side application is required. Open `index.html` in a browser, or serve the project directory locally:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

The page uses inline HTML, CSS, and JavaScript. Google Fonts are loaded remotely as a visual enhancement; system-font fallbacks are provided.

## Demo and pilot status

This repository contains a landing page, not the StudyCircle service itself. Some page sections are explicitly illustrative: the tutor chat is a scripted preview, and the booking and AI retrieval walkthroughs do not connect to payment, tutor, or AI services. The practice diagnostic is interactive, but it uses the page's fixed, hand-written question bank rather than a live AI model.

The pilot sign-up form currently validates the email in the browser and shows a confirmation locally. It does not submit the email to a server or create an actual registration; the selected role and exam or subject are stored in browser `localStorage` when available. No payment is taken.

## Project files

- `index.html` — the complete landing page, including markup, styles, and browser-side interactions.
- `README.md` — project overview and local run instructions.
