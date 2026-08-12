# Biblo — downloads

**Biblo** is a Windows application that reads the PDFs already sitting on your
computer, indexes them locally and lets you question them in plain language:
every answer cites the document and the page it came from.

Website: **https://biblo.app** (also in Italian, French, Spanish and German) ·
**[Download the latest version](../../releases/latest)**

---

## What this repository is

It holds **the downloadable files only**: the Windows installer and the release
notes. Biblo's source code is not public and is not here.

## Installing

1. Download `Biblo_<version>_x64-setup.exe` from the
   [latest release](../../releases/latest).
2. Run it and follow the installer. No administrator rights are needed: Biblo
   installs for your user account.
3. On first launch Biblo asks for a **Cerebras** API key (free) to power the
   AI side.

### Windows will say "Unknown publisher"

The installer is not yet signed with a commercial certificate, so Windows shows
a protection warning the first time you run it. To continue:
**More info** → **Run anyway**.

To confirm you downloaded exactly the file published here, compare the SHA-256
fingerprint (published in every release's notes) with your own copy:

```powershell
(Get-FileHash .\Biblo_1.0.0_x64-setup.exe -Algorithm SHA256).Hash
```

## Requirements

- Windows 10 or 11, 64-bit
- about 2.5 GB of free disk space
- no graphics card: everything runs on the processor
- a Cerebras API key (free tier) for the chat

## Uninstalling

From *Settings → Apps*, or with `uninstall.exe` in the installation folder.
Your PDFs stay where they are: only the application and the data it produced
(`%APPDATA%\Biblo`) are removed.

## Privacy

Documents are indexed on your own computer: no file is uploaded anywhere. When
you ask a question, only the passage needed to answer it is sent to the
language model. Full policy: **https://biblo.app/en/privacy.html**

## Feedback

Problems or suggestions: open an issue in this repository.
