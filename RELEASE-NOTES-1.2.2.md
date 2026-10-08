A small release for anyone setting up Biblo for the first time: the guide to
the free Google Gemini key now shows the whole procedure, including the
welcome Google shows the first time, with a new video. And chats without a
title are now named in the app language.

### Changed

- **The Google Gemini key guide.** The first time you open Google AI Studio,
  Google asks you to accept its terms (you must be 18 or older), then asks
  what brings you there. The guide in Biblo now has five steps that cover
  both, and its video was recorded again from start to finish with a
  brand-new Google account: in English, with subtitles in the five languages
  of the app.

### Fixed

- **"Nuova chat" in every language.** A chat that had no title yet was listed
  as "Nuova chat", in Italian, whatever the language of the app. It is now
  called "New chat" (or the same in your language) in the chat list, in the
  chat details and when you rename it. The automatic title still replaces it
  after the first answer.

### Requirements

- Windows 10 or 11, 64-bit, or a Mac with Apple silicon and macOS 15 or
  later.
- About 2.5 GB of free space; no graphics card needed.
- A free Google Gemini API key (the guide in the app shows how to get one).

Your library, settings and conversations are kept: install over the existing
version. On Windows, Biblo is also available from the Microsoft Store.

On a Mac, Biblo 1.2.0 and later offer this update by themselves and install
it in place. For a new install, open the `.dmg` and drag Biblo into
Applications: the app is signed and notarized by Apple, so it opens with a
double click.

### Verifying the file

| | Windows | Mac |
|---|---|---|
| File | `Biblo_1.2.2_x64-setup.exe` | `Biblo_1.2.2_aarch64.dmg` |
| Size | 565.7 MB (593,153,252 bytes) | 606.2 MB (635,627,447 bytes) |
| SHA-256 | `1AE2E2919484745B1E72374FBF4A48816DE162610532B5BE91CF8E1CCDED428A` | `316DDC61FD145D95194E48633ED05639292DADC26A69CA482E488310D079B221` |

On Windows, in PowerShell:

```powershell
(Get-FileHash .\Biblo_1.2.2_x64-setup.exe -Algorithm SHA256).Hash
```

On a Mac, in Terminal (it prints the same value in lowercase):

```bash
shasum -a 256 Biblo_1.2.2_aarch64.dmg
```
