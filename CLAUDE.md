# model-hub — Projektregeln

Landingpage für zwei getrennte Angebote: Vermittlung von Models an Auftraggeber
und Portfolio-Service für Models. Frankfurt am Main.

Ausführliche Begründungen stehen in @README.md. Diese Datei enthält nur die
Regeln, die beim Arbeiten gelten.

## Regel Nr. 1: Trennung

Vermittlung und Portfolio-Service sind getrennte Angebote.

- Keine Bundles, keine Paketpreise, keine Rabatte für "beides zusammen"
- Portfolio-Service nie als Schritt zur Vermittlung darstellen
- Die Zeile "Für Models kostenlos, bis ein Auftrag zustande kommt" bleibt wörtlich stehen

Grund: Vorschussverbot der Vermittler-Vergütungsverordnung. Verstöße führen zur
Rückzahlungspflicht erhaltener Provisionen.

## Zahlen, die nicht verändert werden dürfen

| Fall | Grenze |
|---|---|
| Engagement bis 7 Tage | 18 % inkl. USt |
| Engagement über 12 Monate | 14 % inkl. USt |

Keine "Verwaltungsgebühr" zusätzlich zur Provision einbauen.

## Textregeln

- Keine hypnotischen Sprachmuster, keine Suggestionstechniken
- Keine Verknappung ("nur noch 3 Plätze"), keine Countdown-Elemente
- Kurze Sätze, keine großen Worte
- Zielgruppe ist teils jung — nichts, was Druck aufbaut

## Datenschutz-Vorgaben

- Zwei getrennte Einwilligungen: Speicherung und Sedcard-Erstellung
- Beide unabhängig widerrufbar
- Upload bleibt freiwillig — die Seite muss ohne Upload funktionieren
- Keine Model-Daten über WhatsApp versenden (Art. 9 DSGVO)
- Bildrechte bleiben beim Model, das steht so auf der Seite

## Farben

| Rolle | Hex |
|---|---|
| Basis Navy | `#0F1B2D` |
| Sektion dunkel | `#16263C` |
| Hintergrund hell | `#F7F4EE` |
| Akzent Vermittlung | `#E8792B` |
| Akzent Portfolio | `#D4A24C` |

Orange gehört zur Vermittlung, Gold zum Portfolio-Service. Diese Zuordnung nicht
mischen — sie macht die Trennung sichtbar.

## Technik

- Eine einzelne `index.html`, CSS inline, kein Build-Schritt, kein Framework
- Icons als Inline-SVG, kein Emoji
- Branch: `main`
- `<meta name="robots" content="noindex, nofollow">` bleibt drin, bis Impressum
  und Datenschutzerklärung live sind

## Was nie ins Repo gehört

Bilder von Models, Verträge, Einwilligungen, PDFs mit Personendaten. Die
`.gitignore` blockt das — aber die Git-History vergisst nichts, also vor jedem
Commit prüfen:

```
git status
```

## Abweichung von den tools-Standardregeln

Regel 9 im tools-Repo lautet "Kein Freelance-/Gewerbe-Framing — André hat kein
Gewerbe". **Für model-hub gilt das nicht.** Die Modelvermittlung ist nach
§ 14 GewO gewerbeanmeldepflichtig. Gewerbliches Framing ist hier korrekt.

## Offen vor Livegang

Siehe Checkliste in @README.md. Die Seite geht nicht live, solange Impressum
und Datenschutzerklärung fehlen — eine öffentlich erreichbare Geschäftsseite
ohne beides ist in Deutschland abmahnfähig.
