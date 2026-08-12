Interface fixes for everyone using Biblo in a language other than Italian.

### Fixed

- **Pipeline steps were always in Italian.** The messages that scroll under
  the answer while Biblo works — *"Searching across languages…"*, *"Generating
  the answer…"* and nine others — were hard-coded in Italian and appeared that
  way in every language. They are now translated into all five.
- **The intent badge showed an internal identifier.** Answers were tagged
  `RIASSUNTO_LIBRO` instead of *Book summary* / *Buchzusammenfassung* /
  *Résumé du livre* / *Resumen del libro*.
- **The assistant's greeting could start in Italian.** In a German or Spanish
  interface the specialised assistant sometimes introduced itself with an
  Italian opening; the greeting is now written entirely in the chosen language.

Nothing else changed: same features, same data, same requirements. Your
library and settings are kept — install over the existing version.

### Verifying the file

| | |
|---|---|
| File | `Biblo_1.0.1_x64-setup.exe` |
| Size | 596.0 MB (624,944,937 bytes) |
| SHA-256 | `6B14A3097D27AC4F5C556B46B6BAA47A77586A9409BEA2D25AB75CC3D870299E` |

```powershell
(Get-FileHash .\Biblo_1.0.1_x64-setup.exe -Algorithm SHA256).Hash
```

### Requirements

Windows 10 or 11, 64-bit · ~2.5 GB free space · no graphics card needed ·
a Cerebras API key (free tier).
