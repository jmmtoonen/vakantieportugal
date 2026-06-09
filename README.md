# Roadtrip Portugal · Porto → Faro

Een interactief, zelfstandig reisplan (één `index.html`, geen build-stap). Met klikbare kaart, route die meereist tijdens het scrollen, en een voorbereidingschecklist die je voortgang lokaal onthoudt.

## Lokaal bekijken
Open `index.html` gewoon in je browser. (Voor de kaarttegels is internet nodig.)

## Op GitHub zetten
```bash
git init
git add index.html README.md
git commit -m "Reisplan Portugal: Porto naar Faro"
git branch -M main
git remote add origin https://github.com/<jouw-gebruikersnaam>/<repo>.git
git push -u origin main
```

## Als Netlify-website publiceren
Twee manieren:

**A. Via GitHub (aanrader, automatische updates)**
1. Ga naar [app.netlify.com](https://app.netlify.com) → **Add new site → Import an existing project**.
2. Kies je GitHub-repo.
3. Build command: *leeg laten*. Publish directory: `.` (de hoofdmap).
4. **Deploy**. Elke `git push` werkt de site daarna automatisch bij.

**B. Slepen en neerzetten (snelst)**
Sleep de map met `index.html` naar het vak op [app.netlify.com/drop](https://app.netlify.com/drop). Klaar.

## Aanpassen
Alle inhoud (haltes, hotels, restaurants, checklist) staat als gewone HTML in `index.html`.
De kaartpunten staan onderin in het `stops`- en `spots`-blok in het script — pas daar coördinaten of namen aan.

Boa viagem! 🇵🇹
