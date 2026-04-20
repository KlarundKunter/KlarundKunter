# KlarundKunter Workflow

## Verbindlicher Session-Start

Jede neue Session fuer KlarundKunter soll mit einer kurzen, nutzerfreundlichen Zusammenfassung beginnen. Diese Formulierung soll aktiv verwendet werden, damit der Workflow fuer den User sofort klar ist.

Verwende zu Beginn jeder neuen Session fuer dieses Repo moeglichst genau diesen Text:

Fuer KlarundKunter arbeiten wir mit einem einfachen Ablauf: Aenderungen entstehen zuerst im Arbeitsstand, werden danach auf der Test-Seite sichtbar geprueft und gehen erst nach ausdruecklicher Freigabe live. So bleibt die Live-Seite stabil, waehrend wir neue Inhalte und Anpassungen in Ruhe auf der Vorschau ansehen koennen.

- `aendere ...` = ich arbeite am Inhalt.
- `zeig auf test` = ich veroeffentliche den aktuellen Stand auf der Test-Seite.
- `Stand von test live nehmen` = ich schiebe den freigegebenen Stand auf live.

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
- Die Session mit dem Text aus "Verbindlicher Session-Start" beginnen.
- Den Starttext nicht nur sinngemaess erwaehnen, sondern moeglichst direkt verwenden.
- Immer knapp bestaetigen, auf welchem Ziel gearbeitet wird: `develop`, `test` oder `live`.
- Keine unnoetigen Tools einfuehren.
- Windows ohne Adminrechte mitdenken.
