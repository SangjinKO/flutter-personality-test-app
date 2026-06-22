# flutter_personality_test

* **Original Repository:** [flutter_personality_test](https://github.com/SangjinKO/flutter_personality_test) *(Private)*

> 💡 **Note:** The link above leads to a private repository used for production. If you need access for evaluation or review, please contact me directly.

Date: 2026.3 - 2026.5

Goal: Develop and publish a cross-platform mobile app for personality tests
- Platform: Flutter, Firebase
- Language: Dart
- Library: firebase_core, firebase_database, firebase_remote_config, firebase_analytics, connectivity_plus
- Tool: Cursor (AI-powered IDE)

Why Flutter:
- First mobile app project — chose Flutter for its single codebase that runs on both iOS and Android
- Dart language combined with Cursor's AI assistance enabled rapid development without prior mobile experience

Includes:
- Main page
  - Shows the list of personality tests loaded from Firebase Realtime Database
  - Pastel-colored card UI with dynamic item height controlled via Remote Config
  - Detects network connectivity and shows an offline notice dialog
- Question page
  - Displays a single scenario-based question per test
  - Multiple radio button choices
- Result page
  - Shows the selected answer and the corresponding personality description
- Firebase integration
  - **Realtime Database**: stores all test content (questions, choices, answers) — new tests can be added anytime without an app update
  - **Remote Config**: controls UI settings (welcome banner on/off, item height) remotely
  - **Analytics**: logs user events (`test_click`, `personal_select`) for usage tracking
