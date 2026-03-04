# Borealise Locales

This repository contains the official localization (i18n) files for
Borealise, a real-time social music platform inspired by classic
social DJ platforms.

Main platform: https://borealise.com

------------------------------------------------------------------------

## 🌍 Purpose

The `locales` repository is responsible for:

-   Storing translation files
-   Managing supported languages
-   Allowing community contributions for new translations
-   Acting as the centralized source for internationalization

These files are consumed by the Borealise frontend and backend to
provide a multilingual experience.

------------------------------------------------------------------------

## 📂 Structure

Each language should have its own JSON file using ISO 639-1 language
codes:

    locales/
    ├── en.json
    ├── pl.json
    ├── pt.json
    └── ...

Example structure inside a locale file:

```json
{
  "common": {
    "welcome": "Welcome",
    "login": "Login",
    "logout": "Logout"
  },
  "room": {
    "join": "Join Room",
    "leave": "Leave Room"
  }
}
```

------------------------------------------------------------------------

## 🛠 Adding a New Language

1.  Copy `en.json` (base language file)
2.  Rename it to your language code (example: `es.json`, `fr.json`)
3.  Translate all values (DO NOT change keys)
4.  Submit a Pull Request

------------------------------------------------------------------------

## ⚠️ Rules

-   Do not change translation keys
-   Do not remove existing fields
-   Keep JSON valid
-   Follow the same nesting structure
-   Keep formatting consistent

If something is unclear, open an issue before making structural changes.

------------------------------------------------------------------------

## 🔄 Updating Translations

When new features are added to Borealise, new keys may appear in
`en.json`.

If you're maintaining a language:
- Add missing keys
- Keep structure identical
- English may be used as fallback until translated

------------------------------------------------------------------------

## 🤝 Contributing

We welcome community contributions.

Steps:

1.  Fork the repository
2.  Create a branch (`feat/add-es-locale` or `fix/pl-typos`)
3.  Commit your changes
4.  Open a Pull Request