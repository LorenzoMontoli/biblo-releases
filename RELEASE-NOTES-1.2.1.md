A small release: Biblo now speaks your language everywhere it still slipped
into Italian, and tells you clearly when the free daily AI quota runs out.

### Fixed

- **Assistants in your language.** The names of the assistants (Aristotle,
  Cicero, Plato…) and their descriptions were shown in Italian whatever the
  language of the app. They now follow the app language, in the chat, on the
  Skills page and in the assistant's greeting. Carolina keeps her name in
  every language, and a name you chose yourself stays yours.
- **The assistant's greeting** no longer addresses you with the assistant's
  own name.
- **Calling an assistant by name** ("Aristotle, summarise…") now works in
  every language, not only in Italian.
- **Smart search** shows its relevance labels and the reason for each result
  in the app language.
- **Selections.** The description Biblo writes for a new selection is now in
  the app language, and says what the documents are about.
- **Improve** keeps your question in the language you wrote it in.
- **Augment search**: its messages, and the headings of the summary it adds
  to the chat, follow the app language.
- **Your own assistants**: the short label Biblo writes for a skill you
  create is in the app language.
- **Daily quota.** When the free daily Google Gemini quota is used up, the
  chat now says so, instead of asking for a key you already have.
- **"Ask the chat about this document"** in the document viewer did nothing.
  Fixed.
- A few remaining Italian labels in other languages (the "Generate with AI"
  button, the Enter key in Help, tooltips on sources, expand/collapse in the
  folder tree, the search counts in the chat's document filter, status
  messages on the Scans and Knowledge pages, connection errors).

### Requirements

- Windows 10 or 11, 64-bit, or a Mac with Apple silicon and macOS 15 or
  later.
- About 2.5 GB of free space; no graphics card needed.
- A free Google Gemini API key (the guide in the app shows how to get one).

Your library, settings and conversations are kept: install over the existing
version. On Windows, Biblo is also available from the Microsoft Store.

### Verifying the file

| | |
|---|---|
| File | `Biblo_1.2.1_x64-setup.exe` |
| Size | 565.5 MB (592,989,958 bytes) |
| SHA-256 | `6F3076285986F1E544880F6B86373DFE1AE9B4DCEE07A494CAE356D45041A1BF` |

```powershell
(Get-FileHash .\Biblo_1.2.1_x64-setup.exe -Algorithm SHA256).Hash
```
