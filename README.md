# Contatore Arrosticini 🍢

Contatore "alla sushi counter" per gli arrosticini: si tocca il contatore al centro, il numero sale di uno e partono i coriandoli. Ai traguardi di **5, 10, 15 e 20** arriva una pioggia di coriandoli extra con un messaggio.

Tutto in un unico file `index.html`: nessuna build, nessuna dipendenza, nessuna installazione.

## Provala in locale

Apri `index.html` nel browser, oppure:

```bash
python3 -m http.server 8000
# poi vai su http://localhost:8000
```

## Pubblicazione su GitHub Pages (2 minuti)

1. Crea un repository nuovo su GitHub (es. `contatore-arrosticini`).
2. Da questa cartella:

   ```bash
   git remote add origin https://github.com/<tuo-utente>/contatore-arrosticini.git
   git branch -M main
   git push -u origin main
   ```

3. Sul repository: **Settings → Pages → Build and deployment**
   - Source: `Deploy from a branch`
   - Branch: `main` / cartella `/ (root)`
   - Salva.

Dopo circa un minuto l'app è online su:

```
https://<tuo-utente>.github.io/contatore-arrosticini/
```

Se il repository si chiama `<tuo-utente>.github.io` l'URL sarà direttamente `https://<tuo-utente>.github.io/`.

## Personalizzare

- **Traguardi e messaggi**: oggetto `MILESTONES` nello `<script>` in fondo a `index.html`.
- **Colori dei coriandoli**: array `PALETTE`.
- **Quantità di coriandoli**: parametro `count` nelle chiamate a `spawn()`.
