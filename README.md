# Mind Bloom

Mind Bloom is a small, browser-based learning and wellbeing game. It turns short moments into playful activities: answer a few questions, match concepts, solve a word puzzle, release a worry, or take a breathing pause. Progress grows a personal flower garden, so learning feels visible without turning the experience into a high-pressure competition.

## Why Mind Bloom?

The project was made to make learning and taking a short mental reset feel approachable. Activities are intentionally brief, can be played at the user's own pace, and reward curiosity rather than streak-chasing. The mood check-in suggests a suitable activity; it is not a diagnosis or a substitute for professional support.

## Features

- Five short activities: Brain Snacks, Concept Pairs, Word Bloom, Pop the Worries, and Slow Breath.
- Urdu and English interface and learning content, with right-to-left layout for Urdu.
- XP, levels, daily quests, badges, streaks, and a plantable flower garden.
- Pip, an animated garden companion.
- Optional, low-volume generated ambient sound with three textures and a volume control.
- Dawn, Garden, Sunset, Midnight, and automatic theme choices.
- Browser-local profile, progress, reviews, and suggestions.
- Six-digit resume-code gate for saved progress on the same browser.
- WhatsApp click-to-chat contact link.

## Technology

Mind Bloom is a single-page static web app built with:

- HTML5 for the app structure.
- CSS3 for responsive styling, themes, animation, and right-to-left Urdu layout.
- Vanilla JavaScript (ECMAScript) for games, localization, audio, progress, and browser interactions.
- Browser Web APIs including `localStorage`, Web Audio API, `MutationObserver`, `Intl.Segmenter` where available, and the Canvas API.
- Google Fonts: Fredoka, Nunito, Noto Nastaliq Urdu, and Noto Sans Arabic.

No framework, package manager, build command, database, or server is required.

## Run Locally

Open `Mind Bloom.html` in a modern browser. An internet connection is used for the hosted Google Fonts; the app itself runs locally, and its sound is generated in the browser.

## Deploy to Vercel

1. Put `index.html`, `Mind Bloom.html`, and this `README.md` in a GitHub repository.
2. In Vercel, import the repository as a **Other** / static project.
3. Leave the build command and output directory empty if Vercel detects the static files automatically.
4. The included `index.html` forwards visitors from the site root to `Mind Bloom.html`.
5. Deploy. No environment variables or API keys are needed for this static version.

## Progress and Resume Codes

The profile, resume-code hash, game progress, and feedback are stored in that browser's `localStorage`. The six-digit resume code verifies access to the saved profile; it does **not** contain or encrypt the save data. It cannot restore progress after site data is cleared, in a different browser/device, or after switching to another deployment origin. For cross-device sync, true account recovery, shared reviews, or secure authentication, connect the app to a backend and database; do not put credentials in the HTML file.

Reviews and suggestions are private to the current browser unless the user chooses to send them through WhatsApp. They are not automatically uploaded or visible to the app owner.

## Language and Accessibility

Use the `اردو` / `English` control in the top bar or **Me → Settings → Language**. Urdu uses right-to-left direction and Urdu-script game content. Reduced-motion preferences are respected. Sound and ambient music are optional and off unless enabled.

## Feedback

Use **Me → Reviews & suggestions** to save feedback locally or open a WhatsApp conversation with the creator. The user chooses whether to send a WhatsApp message.
