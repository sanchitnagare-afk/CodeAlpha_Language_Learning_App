# CodeAlpha_Language_Learning_App
# Bhasha – Language Learning App

An interactive, single-file web app that helps users learn words, phrases and sentences in 10 languages, with translations, pronunciation and quizzes. It runs entirely in the browser and needs no backend.

## Features

- **Flashcards** in three categories: Vocabulary, Phrases and Grammar
- **Translations and pronunciation:** native script, romanized pronunciation and English meaning for every item
- **Listen button** using the browser's Text-to-Speech (Web Speech API)
- **Daily lesson** of 5 items with a streak counter
- **Quiz mode:** 8 multiple-choice questions with scoring and best score per language
- **Progress tracking:** items marked as known, saved locally with `localStorage`
- **Responsive UI** with automatic light and dark mode

## Supported Languages

Hindi, Marathi, Tamil, Telugu, Bengali, Gujarati, Kannada, Malayalam, Spanish, French

## Tech Stack

- HTML5
- CSS3 (CSS variables, flexbox)
- Vanilla JavaScript
- Web Speech API
- localStorage for data storage

## Project Structure

```
bhasha-language-learning-app/
├── index.html    # HTML, CSS and JavaScript in one file
└── README.md
```

## How to Run

1. Clone or download this repository:
   ```bash
   git clone https://github.com/<your-username>/bhasha-language-learning-app.git
   ```
2. Open `index.html` in any modern browser (Chrome, Edge, Safari or Firefox).

No installation or build step is required.

## How It Works

| Tab | What it does |
|-----|--------------|
| Learn | Flip cards by category, listen to pronunciation, mark items as known |
| Daily | Shows 5 new items each day and tracks your streak |
| Quiz | Tests your learning with multiple-choice questions |
| Progress | Shows known items, best quiz scores and streak for each language |

## Adding a New Language

Add an entry to the `L` object in the script:

```js
pa: {
  n: "Punjabi",
  v: "pa-IN",                      // voice code for text-to-speech
  t: "Grammar tip for this language.",
  w: [
    ["Water", "ਪਾਣੀ", "paani"],    // [English, Native script, Pronunciation]
    // 12 items: 5 vocabulary, 5 phrases, 2 grammar sentences
  ]
}
```

## Notes

- Audio depends on the voices installed on the user's device. Some languages may have no voice on certain browsers.
- Progress is stored in the browser, so clearing site data resets it.

## Future Improvements

- More languages and lessons
- Firebase login and cloud sync
- Spaced repetition for reviewing cards
- Fill-in-the-blank and listening quizzes
