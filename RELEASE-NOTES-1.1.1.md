A maintenance release: a new PDF reading engine, a smaller download, and a
privacy policy that describes what the app actually does.

### Changed

- **New PDF engine.** Document reading now uses PDFium (the engine behind Google
  Chrome) instead of the previous library. Text extraction is slightly more
  accurate — titles set with letter spacing are now read as words rather than
  as separate letters, which makes searching them work — and the download is
  **31 MB smaller**.
  ⚠️ **If you want the improved extraction applied to documents you have already
  read, read them again** from the Library page. Existing documents keep
  working as they are; scanned documents are unaffected, because their text
  comes from the OCR pass and has not changed.
- **Clearer privacy policy and terms.** The previous wording suggested the app
  might come with API keys provided by us. It does not, and never has since the
  key setup screen was introduced: the app ships with **no keys**, every AI
  request runs through *your* key and *your* account with Mistral or Google.
  That is not a wording detail — it decides who is responsible for your data
  under the GDPR — so the documents now say plainly that for the documents you
  index and the questions you ask **you** are the data controller, and that we
  are controllers only for this website, purchases and support. The sections on
  providers, international transfers, legal basis and retention were corrected
  to match, and the free-tier warnings are now explicit (Google's unpaid tier
  asks you not to submit confidential information and its human reviewers may
  read API traffic; on Mistral, training on your data is on by default and must
  be switched off in your account).
  **You will be asked to review and accept the updated documents once.**

### Requirements

Windows 10 or 11, 64-bit · ~2.5 GB free space · no graphics card needed ·
a Mistral AI **or** Google Gemini API key (free tier — one is enough).

Your library, settings and conversations are kept — install over the existing
version.

### Verifying the file

| | |
|---|---|
| File | `Biblo_1.1.1_x64-setup.exe` |
| Size | 585.9 MB (614,320,436 bytes) — 11 MB smaller than 1.1.0 |
| SHA-256 | `817F3557C3D06F6F312C4A09255762A3B3B6345A6C26D9E12399AAC15E6F6E0A` |

```powershell
(Get-FileHash .\Biblo_1.1.1_x64-setup.exe -Algorithm SHA256).Hash
```
