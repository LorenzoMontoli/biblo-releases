A bigger release: Biblo now runs on Mac too, uses a single free Google
Gemini key for everything, and shows you step by step (with a short video)
how to get that key. It also fixes several problems that only appeared in the
installed app.

### New

- **Biblo for Mac.** The same app, with the same features, now runs on Macs
  with Apple silicon. The Mac download is part of this release, next to the
  Windows installer.
- **One AI service: Google Gemini.** Chat, Improve, smart search, Inspect and
  Find connections all run on one free Google Gemini key. Mistral is no longer
  supported: if you only had a Mistral key, Biblo will ask for a Gemini key
  the first time you use an AI feature. Your documents, library and
  conversations are not affected.
- **Getting the key, explained.** Until a key is set, Biblo shows a reminder
  at startup with a step-by-step guide and a 20-second video, subtitled in
  English, Italian, French, Spanish and German. It never blocks you:
  importing, reading and searching your documents work without any key, and
  "Continue without a key" closes it. Keys are checked with Google before
  being saved, and problems are explained in your language.
- **Updates from inside the app.** When a new version comes out, Biblo
  offers to download and install it, showing the progress. The package's
  signature is checked before anything is installed.
- **Report button** under every AI answer: it opens a pre-filled email so you
  can tell us about a wrong or inappropriate answer. Nothing is sent unless
  you send that email yourself.
- **"Choose folder"** in the first setup opens the system folder picker, so
  you don't have to type a path.

### Fixed

- **Chat on new installations.** On a fresh install the chat could answer
  that a "Cerebras API key" was missing, even with a valid key. Fixed.
- **Confirmations.** "Delete all" in Chat deleted every conversation
  without asking, and the other confirmations (moving a document to the
  Recycle Bin, removing a folder from the library) went ahead without asking
  too. They now ask, and Cancel really cancels.
- **Links** to create your key, and the download link of the "new version"
  notice, now open in your browser.
- **Uninstalling** with "Delete the application data" ticked now removes
  your library index, conversations and settings too; before, they stayed on
  the disk. Without the box ticked they are kept, as before.
- **Key fields no longer remember what you type**, so previously entered
  keys are never offered as suggestions.
- **Closing Biblo from Task Manager** no longer leaves its background process
  running.
- **Smaller download**: 20 MB smaller than 1.1.1 (two unused
  scientific libraries removed).

### Privacy policy and terms

Updated (version 4) to describe this version: Google Gemini as the only AI
service, with the conditions of its free tier, and the connections to GitHub
that check for and download updates. **You will be asked to review and
accept them once.**

### Requirements

- Windows 10 or 11, 64-bit, or a Mac with Apple silicon and macOS 15 or
  later.
- About 2.5 GB of free space; no graphics card needed.
- A free Google Gemini API key (the guide in the app shows how to get one).

Your library, settings and conversations are kept: install over the existing
version.

On a Mac, open the `.dmg` and drag Biblo into Applications. The app is
signed and notarized by Apple, so it opens with a double click: macOS only
asks once whether to open an app downloaded from the internet.

### Verifying the file

| | Windows | Mac |
|---|---|---|
| File | `Biblo_1.2.0_x64-setup.exe` | `Biblo_1.2.0_aarch64.dmg` |
| Size | 565.5 MB (592,948,479 bytes) — 20 MB smaller than 1.1.1 | 606.0 MB (635,443,646 bytes) |
| SHA-256 | `E04E6D4D00BA388F16AA8AA6178D2C760DABBC09DE6A91D4A4143FE5C0EE7C5F` | `A2B2F92B41EE35603876DD1C0B16529C65258C0D4F0C9DB8B47E2F07D5C90DA3` |

On Windows, in PowerShell:

```powershell
(Get-FileHash .\Biblo_1.2.0_x64-setup.exe -Algorithm SHA256).Hash
```

On a Mac, in Terminal (it prints the same value in lowercase):

```bash
shasum -a 256 Biblo_1.2.0_aarch64.dmg
```
