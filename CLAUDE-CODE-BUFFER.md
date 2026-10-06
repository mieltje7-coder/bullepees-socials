# Bullepees → Buffer: instructie voor Claude Code

## Koppelen (eenmalig)
```
claude mcp add --transport http buffer https://mcp.buffer.com/mcp --header "Authorization: Bearer JOUW_BUFFER_API_KEY"
```
API-key: Buffer → Settings → API. Deel of commit deze key nooit.

## Wat er klaarstaat
- `buffer-posts.json` → 15 posts (13 feed, 2 stories) met datum/tijd (Europe/Amsterdam), caption, hashtags, link en bestandsnamen.
- `pNN-N.png` / `sNN-N.png` → de afbeeldingen. Feed 1080×1080 of 1080×1350, stories 1080×1920.
- Carrousels: `p02`, `p07`, `p09` (3 afbeeldingen), `p04` (2) en de blog `p05` (6). Story `s01` heeft 3 frames. Upload altijd in volgorde 1-2-3.

## Opdracht voor Claude Code
> Lees `export/buffer-posts.json`. Maak voor elke post een **draft** in Buffer op de Instagram- en Facebook-kanalen van Bullepees, op de opgegeven datum en tijd. Caption = `caption` + twee enters + `hashtags`. Voeg de afbeeldingen uit `images` toe (in volgorde). Stories: zonder caption, en zet de `sticker`-link in de notitie. Publiceer niets direct. Geef daarna een overzicht van wat er is aangemaakt.

## Let op
- Buffer heeft voor afbeeldingen een **publieke URL** nodig. Zet de PNG's eerst online (bijv. in de mediabibliotheek van bullepees.nl of een gedeelde map) en vervang de paden in `images` door die URL's, of upload de afbeeldingen handmatig bij de drafts.
- Feed-posts op Instagram hebben geen klikbare link; daarom staat er "link in bio". Zet in je bio de link naar bullepees.nl.
- Link-stickers in stories voeg je toe in de Instagram-app als Buffer een herinnering stuurt.
- Controleer elke draft voordat je hem inplant.
