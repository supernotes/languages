# Supernotes Community Translations

Community-contributed translation files for [Supernotes](https://supernotes.app), the collaborative note-taking and knowledge management app.

![3 2 2](https://github.com/user-attachments/assets/76ceb7f9-193a-44a1-8425-28854be209e8)


## Available Languages

| Flag | Language | Code | Status |
|------|----------|------|--------|
| 🇬🇧 | English | `en` | Source |
| 🇬🇧 | English (UK) | `en-gb` | Complete |
| 🇩🇪 | German | `de` | Complete |
| 🇪🇸 | Spanish | `es` | Complete |
| 🇫🇷 | French | `fr` | Complete |
| 🇮🇩 | Indonesian | `id` | Complete |
| 🇮🇹 | Italian | `it` | Complete |
| 🇵🇹 | Portuguese | `pt` | Complete |
| 🇧🇷 | Portuguese (Brazil) | `pt-br` | Complete |

## File Structure

Each locale is a single JSON file named `<locale-code>.json`. Files use a nested key structure:

```json
{
  "_lang_code": "fr",
  "_lang_english": "French",
  "_lang_native": "Français",
  "_lang_flag": "🇫🇷",
  "actions": {
    "archive": "Archiver",
    "cancel": "Annuler",
    ...
  },
  ...
}
```

The `_lang_*` metadata keys at the top of each file define the locale's display name, native name, and flag emoji.

## Contributing

We welcome translations for new languages and improvements to existing ones!

### Improving an Existing Translation

1. Open the relevant `<locale-code>.json` file
2. Find the key(s) you'd like to improve
3. Submit a pull request with your changes

### Adding a New Language

1. Copy `en.json` as a starting point
2. Rename it to your [BCP 47 language tag](https://en.wikipedia.org/wiki/IETF_language_tag) (e.g. `ja.json`, `ko.json`, `zh-cn.json`)
3. Update the `_lang_code`, `_lang_english`, `_lang_native`, and `_lang_flag` metadata fields
4. Translate all values (keys must stay the same)
5. Submit a pull request

### Translation Guidelines

- **Preserve placeholders** like `{{count}}`, `{{name}}`, `{{price}}` exactly as they are
- **Preserve HTML tags** like `<bold>`, `<red>`, `<italic>`, `<b>`, `<kbd>` exactly as they are
- **Keep product names in English:** Supernotes, Anti-Procrastin, Noteboard
- **Keep technical terms** where appropriate: markdown, JSON, PDF, API, LaTeX
- **Empty strings should stay empty** (e.g. `"tips.empty": ""`)
- All keys present in `en.json` must be present in your translation (100% coverage required)

## License

These translations are provided for use with [Supernotes](https://supernotes.app). All rights reserved by Supernotes Ltd.
