# LIBRO

Raccolta testuale del progetto narrativo ambientato nel mondo di Aldarion. Il repository contiene capitoli, schede personaggi, mappe concettuali, canzoni e documenti di analisi e miglioramento.

## Obiettivi
- Centralizzare tutti i materiali testuali.
- Versionare in modo atomico le modifiche (commit piccoli e descrittivi).
- Facilitare revisione, refactoring narrativo e tracciamento dell'evoluzione.

## Struttura
- `capitoli/` capitoli correnti numerati in ordine di lettura.
- `vecchi capitoli/` versioni precedenti o scartate (storia evolutiva).
- `character/` schede personaggi, famiglie, fazioni.
- `canzoni/` testi di canzoni o componimenti poetici integrati nella lore.
- `scaletta/` scalette, outline e pianificazioni.
- `MAPPA_ALDARION.md` mappa concettuale del mondo.
- `ANALISI_CRITICITA_AETHERNITAS.md` analisi criticità.
- `PIANO_MIGLIORAMENTO_10_10.md` piano di miglioramento qualitativo.
- `piano_integrazione_personaggi_secondari.md` strategia per integrazione cast.
- `sistema_dialetti_regionali.md` regole dialettali e linguistiche.
- `character_vocal_patterns.md` coerenza voci e pattern espressivi.
- `.gitignore` configurazione esclusioni.

## Convenzioni di scrittura
- File di testo in UTF-8 senza BOM.
- Nomi file minuscoli con spazi solo dove esplicitamente utile alla leggibilità.
- Evitare caratteri speciali non ASCII nei nomi di file (accenti) per portabilità.
- Ogni capitolo in un file separato, prefisso "capitolo N".
- Aggiornare le schede personaggio quando un evento modifica tratti o relazioni.

## Convenzioni Git
- Commit frequenti (idealmente per capitolo o modifica coerente).
- Messaggio commit formato: `tipo: breve descrizione` dove tipo può essere:
  - `chap` nuovo capitolo o modifica sostanziale
  - `char` aggiornamento scheda personaggio
  - `lore` documentazione mondo / sistemi
  - `refac` ristrutturazione / rinomina file
  - `fix` correzioni minori (refusi, punteggiatura)
- Esempio: `chap: revisione dialoghi capitolo 5`

## Flusso di lavoro suggerito
1. Creare un branch se la revisione è ampia: `git checkout -b revisione-cap5`.
2. Applicare modifiche incrementali.
3. Eseguire `git add` mirato (evitare `git add .` se non necessario).
4. Commit chiari.
5. Merge sul branch principale quando la revisione è completa.

## Creazione repository remoto (manuale via interfaccia web)
1. Apri GitHub e crea una nuova repository (nome suggerito: `libro-aldarion`).
2. NON inizializzare con README / .gitignore su GitHub (già presenti localmente).
3. Copia l'URL remoto (HTTPS o SSH).
4. In locale esegui:
   - HTTPS: `git remote add origin https://github.com/UTENTE/libro-aldarion.git`
   - Oppure SSH: `git remote add origin git@github.com:UTENTE/libro-aldarion.git`
5. Imposta il branch principale (se non esiste già): `git branch -M main`
6. Primo push: `git push -u origin main`

## Installazione opzionale GitHub CLI
Se desideri automatizzare passi futuri:
- Scarica da: https://cli.github.com/
- Dopo l'installazione: `gh auth login`

## Prossimi passi immediati
- Aggiungere tutti i file e creare commit iniziale.
- Creare repository remoto e pubblicare.
- Pianificare prossima iterazione di revisione (vedi piani allegati).

## Licenza / visibilità
Decidere se repository sarà privato o pubblico prima del push. Se privato, verificare di non includere materiale sensibile in commit futuri.

---
Ultimo aggiornamento iniziale del README.