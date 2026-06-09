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

## Foto's
De foto's per bestemming komen van **Wikimedia Commons** en worden geladen via de stabiele `Special:FilePath`-link, zodat ze niet snel breken. Ze staan in het `PHOTOS`-blok onder in `index.html` (per stop een bestandsnaam + bijschrift). Wil je een foto vervangen, zoek dan een bestand op [commons.wikimedia.org](https://commons.wikimedia.org) en zet de exacte bestandsnaam in de lijst.

De meeste Commons-foto's vallen onder een Creative Commons-licentie (vaak met naamsvermelding). Voor een persoonlijke reispagina is dat prima; wil je het helemaal netjes of commercieel gebruiken, vervang ze dan door je eigen foto's of voeg per foto de maker + licentie toe.

Boa viagem! 🇵🇹
