# KlarundKunter Workflow

## Session Start Summary

Zu Beginn jeder neuen Session soll diese Kurzfassung gezeigt und beachtet werden:

- Repo: `KlarundKunter/KlarundKunter`
- Arbeitsbranch: `develop`
- Live-Branch: `main`
- Sichtbare Vorschau: `test.klarundkunter.de`
- Produktion: `klarundkunter.de`
- Umgebung: Windows lokal, kein Adminzugang
- Ziel: so wenig Tooling wie moeglich, moeglichst viel operativ durch Codex

## Arbeitsregeln

1. Neue Aenderungen entstehen zuerst im Repo `KlarundKunter` auf `develop`.
2. Wenn ein Stand sichtbar geprueft werden soll, wird der aktuelle Stand nach `test.klarundkunter.de` uebernommen und dort veroeffentlicht.
3. `main` und `klarundkunter.de` bleiben unveraendert, bis eine ausdrueckliche Freigabe kommt.
4. Wenn die Anweisung lautet `Stand von test live nehmen`, wird genau der gepruefte Stand sauber nach `main` uebernommen und damit auf `klarundkunter.de` live gestellt.

## Operative Bedeutung

- `aendere ...` bedeutet: auf `develop` arbeiten
- `zeig auf test` bedeutet: Stand nach `test.klarundkunter.de` veroeffentlichen
- `Stand von test live nehmen` bedeutet: den freigegebenen Teststand nach Produktion uebernehmen

## Technische Struktur

- Arbeitsrepo: `KlarundKunter`
- Staging-Repo: `test.klarundkunter.de`
- Produktionsauslieferung: GitHub Pages fuer `main`
- Staging-Auslieferung: GitHub Pages fuer `test.klarundkunter.de`

## Hinweise fuer neue Sessions

- Zuerst diese Datei lesen.
- Die Session mit der "Session Start Summary" beginnen.
- Immer knapp bestaetigen, auf welchem Ziel gearbeitet wird: `develop`, `test` oder `live`.
- Keine unnoetigen Tools einfuehren.
- Windows ohne Adminrechte mitdenken.
