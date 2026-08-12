# Biblo — download

**Biblo** è un'applicazione per Windows che legge i PDF che hai già sul
computer, li indicizza in locale e ti lascia interrogarli in linguaggio
naturale: ogni risposta cita il documento e la pagina da cui viene.

Sito: **https://biblo.app** · Scarica: **[ultima versione](../../releases/latest)**

---

## Che cos'è questo repository

Contiene **solo i file da scaricare**: l'installatore di Windows e le note di
rilascio. Il codice sorgente di Biblo non è pubblico e non si trova qui.

## Installazione

1. Scarica `Biblo_<versione>_x64-setup.exe` dall'[ultima release](../../releases/latest).
2. Aprilo e segui l'installazione. Non servono permessi di amministratore:
   l'applicazione si installa per il tuo utente.
3. Al primo avvio Biblo ti chiede una chiave **Cerebras** (gratuita) per la
   parte di intelligenza artificiale.

### Windows dirà «Autore sconosciuto»

L'installatore non è ancora firmato con un certificato commerciale, quindi
Windows mostra un avviso di protezione al primo avvio. Per procedere:
**Ulteriori informazioni** → **Esegui comunque**.

Se vuoi verificare di avere scaricato esattamente il file pubblicato qui,
confronta l'impronta SHA-256 (la trovi nelle note di ogni release) con quella
del tuo file:

```powershell
(Get-FileHash .\Biblo_1.0.0_x64-setup.exe -Algorithm SHA256).Hash
```

## Requisiti

- Windows 10 o 11 a 64 bit
- circa 2,5 GB di spazio su disco
- nessuna scheda grafica: tutto gira sul processore
- una chiave Cerebras (piano gratuito) per la chat

## Disinstallazione

Da *Impostazioni → App*, oppure con `uninstall.exe` nella cartella di
installazione. I tuoi PDF restano dove sono: vengono rimossi solo
l'applicazione e i dati che ha prodotto lei (`%APPDATA%\Biblo`).

## Privacy

L'indicizzazione dei documenti avviene sul tuo computer: i file non vengono
caricati da nessuna parte. Quando fai una domanda, al modello linguistico
viene inviato solo il brano necessario a rispondere.
Informativa completa: **https://biblo.app/it/privacy.html**

## Segnalazioni

Problemi o proposte: apri una *issue* in questo repository.
