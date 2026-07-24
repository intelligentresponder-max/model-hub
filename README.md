# model-hub

Landingpage für zwei getrennte Angebote: Vermittlung von Models an Auftraggeber
und Portfolio-Service für Models. Frankfurt am Main.

**Status:** In Aufbau. Seite steht auf `noindex`. Nicht live gehen, bevor die
offenen Punkte unten abgearbeitet sind.

---

## Die Trennungsregel

Das ist die wichtigste Regel im ganzen Projekt.

**Vermittlung und Portfolio-Service sind getrennte Angebote.** Getrennte
Verträge, getrennte Rechnungen. Das eine ist nie Voraussetzung für das andere.

Grund: Fotomodelle sind in der Vermittler-Vergütungsverordnung namentlich
aufgeführt (§ 1: „Fotomodell, Werbetyp, Mannequin und Dressman"). Wenn ein Model
erst einen Portfolio-Service kauft und danach vermittelt wird, kann das als
Vorschuss auf die Vermittlungsleistung gewertet werden — und Vorschüsse sind
verboten. Gerichte haben Agenturen deshalb zur Rückzahlung erhaltener
Provisionen verurteilt, auch nach Jahren erbrachter Leistung (Nichtigkeit nach
§ 134 BGB).

Konkret heißt das für Texte auf der Seite:

- Kein Bundle, kein Paketpreis, keine Rabatte für „beides zusammen"
- Der Portfolio-Service darf nirgends als Schritt zur Vermittlung dargestellt werden
- Die Zeile „Für Models kostenlos, bis ein Auftrag zustande kommt" bleibt so stehen

---

## Rechtliche Eckpunkte

### Vergütung (Vermittlungszweig)

| Fall | Obergrenze |
|---|---|
| Engagement bis 7 Tage | 18 % des Modelhonorars |
| Engagement über 12 Monate | 14 % des Modelhonorars |

Jeweils **einschließlich Umsatzsteuer**. Die Grenze gilt auch bei Zusammenarbeit
mit anderen Vermittlern.

Eine „Verwaltungsgebühr" zusätzlich zur Provision ist der übliche Umgehungsweg —
und genau der, der vor Gericht kassiert wird. Nicht machen.

### Weitere Vorgaben

- **Schriftform Pflicht.** Mündliche Vereinbarungen über Vermittlung und
  Vergütung sind unwirksam (§ 296 Abs. 1, § 297 Nr. 1 SGB III).
- **Keine Vorschüsse** auf die Vermittlungsvergütung.
- **Kein Exklusivvertrag.** Exklusivbindungen ohne klare Eingrenzung gelten als
  Knebelung (§ 138 BGB).
- **Gewerbeanmeldung** nach § 14 GewO ist Pflicht.
- **Grenze zur Arbeitnehmerüberlassung:** Sobald aktiv Verträge ausgehandelt
  werden oder als Produktionspartner aufgetreten wird, greift § 1 AÜG — dann
  erlaubnispflichtig.

### Offene Risiken, noch nicht geklärt

- **Künstlersozialabgabe** (§ 24 KSVG) — kann greifen, sobald regelmäßig
  künstlerische Leistungen eingekauft werden (z. B. Sedcard-Shootings)
- **Scheinselbstständigkeit** (§ 611a BGB) — bei Models, die regelmäßig
  weisungsgebunden arbeiten. Folge: Nachforderungen der Sozialversicherung,
  im Extremfall § 266a StGB

---

## Kontaktwege

Hauptweg sind zwei **WhatsApp-Direktlinks** (`wa.me`), einer je Angebot. Klick
öffnet einen Einzelchat mit vorformuliertem Text:

| Button | Vorformulierter Text |
|---|---|
| Vermittlung (orange) | „Hallo, ich interessiere mich für die Vermittlung." |
| Portfolio-Service (gold) | „Hallo, ich interessiere mich für den Portfolio-Service." |

So ist beim Eingang sofort erkennbar, aus welchem Zweig die Anfrage kommt.

**Bewusst keine WhatsApp-Gruppe.** In einer Gruppe sehen alle Mitglieder die
Telefonnummern aller anderen. Bei einer Zielgruppe aus teils jungen Menschen
wäre ein öffentlich verlinkter Gruppen-Einladungslink ein Datenleck by design.
Der Direktlink hat dieses Problem nicht.

**Über WhatsApp laufen keine Bilder.** Die Zeile „Bilder bitte nicht über
WhatsApp senden — dafür melden wir uns per E-Mail" steht aus einem Grund auf der
Seite: Modeldaten fallen unter Art. 9 DSGVO, WhatsApp ist dafür nicht geeignet.
Die Zeile dokumentiert außerdem, dass ungefragt zugesandte Fotos nicht
erwünscht waren. Nicht entfernen.

E-Mail steht als zweiter Weg darunter.

---

## Datenschutz

Modeldaten (Fotos, Maße, Sedcards) fallen unter **Art. 9 DSGVO** — besondere
Kategorien personenbezogener Daten. Entsprechend höhere Anforderungen.

### Einwilligungs-Logik

Zwei **getrennte** Einwilligungen, unabhängig voneinander widerrufbar:

1. **Speicherung** der hochgeladenen Bilder
2. **Erstellung einer Sedcard** durch uns (nur wenn explizit freigegeben)

Ein Widerruf der Sedcard-Einwilligung berührt die Vermittlung nicht. Ein
Widerruf der Speicherung führt zur Löschung.

Einwilligungen dürfen **nicht** im allgemeinen Vertrag versteckt werden. Sie
müssen eigenständig dokumentiert werden (Rechenschaftspflicht, Art. 5 Abs. 2
DSGVO).

### Bildrechte

Die Agentur erwirbt **keine** Nutzungsrechte durch den Upload. Das Model behält
alle Rechte. Für jede Verwendung wird separat gefragt.

Vor Weitergabe von Material an Dritte (Marken, Magazine, Plattformen) besteht
eine Prüfpflicht. Fehlende Rechteklärung kann Schadensersatz nach § 97 UrhG
auslösen.

### Google Drive

Der Upload läuft vorerst über Google Drive. Dafür gilt:

- **Google Workspace nötig**, kein privates Konto — nur dort lässt sich der
  Zusatz zur Datenverarbeitung (AVV) abschließen
- Adminkonsole → Konto → Kontoeinstellungen → Zusatz anzeigen → bestätigen
- Ohne diesen Schritt kein wirksamer AVV nach Art. 28 DSGVO

**Bekannte Schwäche:** Drive hat kein Rechtemanagement pro Person, keine
Löschprotokolle, und Links werden leicht weitergereicht. Für Art.-9-Daten
grenzwertig. Umstieg auf eine geeignetere Lösung einplanen.

---

## Aufbau

```
model-hub/
├── index.html      Landingpage (single file, CSS inline)
├── CLAUDE.md       Projektregeln für Claude Code
├── README.md       Diese Datei
└── .gitignore
```

Kein Build-Schritt, kein Framework. Die Seite ist eine einzelne HTML-Datei mit
eingebettetem CSS und einem kleinen Scroll-Reveal-Script.

### Design

| Rolle | Wert |
|---|---|
| Basis | `#0F1B2D` (Navy) |
| Sektion dunkel | `#16263C` |
| Hintergrund hell | `#F7F4EE` (Cream) |
| Akzent Vermittlung | `#E8792B` (Orange) |
| Akzent Portfolio | `#D4A24C` (Gold) |

Die Farbtrennung ist Absicht: Orange steht für den Vermittlungszweig, Gold für
den Portfolio-Service. Das unterstützt visuell, was rechtlich gelten muss.

Alle Icons sind Inline-SVG, kein Emoji — rendert geräteunabhängig identisch.

---

## Offene Punkte vor dem Livegang

- [x] WhatsApp-Direktlinks eingebaut (beide Zweige, vorformulierter Text)
- [ ] E-Mail-Adresse eintragen (aktuell `PLATZHALTER@DOMAIN.DE` in `index.html`)
- [ ] Impressum schreiben und verlinken
- [ ] Datenschutzerklärung schreiben und verlinken
- [ ] AGB schreiben und verlinken
- [ ] Galerie-Bilder einsetzen (7 Slots, `.ph`-Divs durch `<img>` ersetzen)
- [ ] Google Workspace einrichten und AVV-Zusatz bestätigen
- [ ] Vertragsmuster anwaltlich prüfen lassen — **beide Zweige getrennt**
- [ ] Einwilligungstexte anwaltlich prüfen lassen
- [ ] Gewerbe anmelden
- [ ] `noindex` entfernen (erst wenn alles obige steht)

---

## Textregeln

- Keine hypnotischen Sprachmuster, keine Suggestionstechniken. Eine Einwilligung
  muss freiwillig und informiert sein — Trance-Sprache untergräbt genau das.
- Keine Verknappung („nur noch 3 Plätze"), keine Countdown-Elemente.
- Kurze Sätze. Die Ruhe ist bei diesem Thema das bessere Verkaufsargument.
- Zielgruppe ist teils jung. Nichts, was Druck aufbaut.

---

## Hinweis

Die rechtlichen Angaben in dieser Datei stammen aus eigener Recherche, nicht aus
anwaltlicher Beratung. Vor dem Livegang gehört alles einmal von einem Anwalt
geprüft — besonders die Vertragsmuster und die Einwilligungstexte.

Quellen: VermittVergV §§ 1–2, SGB III §§ 296–301, DSGVO Art. 5/9/28, GewO § 14,
AÜG § 1, UrhG § 97.
