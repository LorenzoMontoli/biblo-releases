Biblo now speaks to two AI providers — Mistral AI and Google Gemini — replacing Cerebras, whose free tier was discontinued. One free key from either provider is enough.

### Changed

- **New AI providers: Mistral AI and Google Gemini.** Cerebras turned its free
  tier into a 30-day trial, so Biblo moved to two providers with real free
  plans. One key is enough; with both, Biblo splits the work between them and
  falls back to the other when one is busy.
  ⚠️ **Existing Cerebras keys no longer work**: on first launch the app asks
  for a Mistral or Gemini key (free, takes a minute to obtain — the setup
  screen links to both and explains the pros and cons of each, including how
  each provider treats your data).
- **Updated privacy policy and terms.** The documents now describe the new
  providers, so the app asks everyone to review and accept them once.

### Added

- **Math formulas in chat.** Scientific texts make the model produce LaTeX;
  answers now render it properly instead of showing raw markup.
- **Wait-time estimates.** Every AI operation shows a small banner with the
  estimated duration, so you know whether to wait or come back later. It can
  be turned off from the banner itself or in Settings → Appearance.
- **Chat titles in your language.** Conversation titles are generated in the
  language of your question; progress messages follow the app language.

### Fixed

- **Chat stays alive while reading documents.** Asking questions during
  indexing no longer waits for the indexer to finish.
- **Accented characters in streamed answers.** Answers could show garbled
  accents (e.g. "stabilitÃ " instead of "stabilità"); streams are now decoded
  correctly in all languages.
- **PDFs with a broken extension are recovered** instead of being skipped.
- **Sturdier reading on low-memory machines**, with a safeguard against
  out-of-memory failures during document reading.

Your library, settings and conversations are kept — install over the existing
version.

### Verifying the file

| | |
|---|---|
| File | `Biblo_1.1.0_x64-setup.exe` |
| Size | 596.7 MB (625,692,987 bytes) |
| SHA-256 | `BC3E52F4CE0E8BB5E2A348FFE4FA3F479B136A5517DAEE69193F1931B718B155` |

```powershell
(Get-FileHash .\Biblo_1.1.0_x64-setup.exe -Algorithm SHA256).Hash
```

### Requirements

Windows 10 or 11, 64-bit · ~2.5 GB free space · no graphics card needed ·
a Mistral AI **or** Google Gemini API key (free tier — one is enough).
