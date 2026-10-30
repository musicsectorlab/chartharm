# Sito di ChartHarm (privacy e assistenza)

Pagine statiche da mettere online, richieste dall'App Store:

| File | Uso in App Store Connect |
|---|---|
| `privacy.html` | **URL della privacy** (obbligatorio) |
| `support.html` | **URL di assistenza** (obbligatorio) |
| `index.html` | URL di marketing (facoltativo) |

Ogni pagina è in italiano e in inglese. `style.css`, `icona.png` e `schermata.jpg` vanno caricati insieme alle pagine; `LEGGIMI.md` non va messo online.

## Pubblicare gratis con GitHub Pages
Come per StageLab e ChartLab, con l'account `musicsectorlab`:

1. Su **github.com** scegli **New repository**, come nome scrivi `chartharm`, seleziona *Public* e premi **Create repository**.
2. Scegli **uploading an existing file**, trascina i file di questa cartella (tranne `LEGGIMI.md`) e premi **Commit changes**.
3. In **Settings › Pages** imposta *Branch* `main` e la cartella `/ (root)`, poi premi **Save**.
4. Dopo circa un minuto il sito è online:
   - privacy: `https://musicsectorlab.github.io/chartharm/privacy.html`
   - assistenza: `https://musicsectorlab.github.io/chartharm/support.html`

Gli stessi indirizzi sono già nell'app (Impostazioni › Informazioni › Privacy e Assistenza): se il repository ha un altro nome, vanno cambiati anche in `ChordScope/Views/LiveAndTunerViews.swift`.

In **App Store Connect** vanno in *Informazioni app › URL della privacy* e *URL di assistenza*.

## Da aggiornare se cambia l'app
- **Versione gratuita:** se cambia il limite di 3 brani, aggiornalo in `support.html` (italiano e inglese).
- **Modello del testo:** se cambia il modello predefinito o la sua dimensione, aggiorna `support.html`; se cambia da dove si scarica (oggi Hugging Face), aggiorna `privacy.html`.
- **Lingua:** l'app è solo in italiano; quando arriva l'inglese, togli la frase "The app is currently in Italian" da `support.html`.
- Se cambia l'informativa, aggiorna anche la data in cima a `privacy.html`.
