# UmfragePortal – Phishing-Aufklärung für den Schulunterricht

> ⚠️ **DISCLAIMER: Dies ist KEINE echte Umfrage und KEINE echte Phishing-Seite.**
> Es handelt sich um eine harmlose Lern-Demo für den Unterricht in Medien & Informatik.

## Worum geht es?

Diese Seite simuliert ein seriös wirkendes Umfrage-Portal mit einer verlockenden
Belohnung («Fr. 10.– nach Abschluss»). Wer sich «einloggt», sieht sofort eine
Aufklärungsseite («YOU HAVE BEEN PHISHED!») mit Tipps, wie man Phishing erkennt.

Ziel ist, dass Schülerinnen und Schüler am eigenen Beispiel erleben, wie leicht man
auf eine professionell aussehende Seite hereinfällt – in einem geschützten Rahmen.

## Datenschutz & Sicherheit

- **Es werden keine Daten gespeichert oder übertragen.** Die Seite läuft komplett im
  Browser (eine einzige statische HTML-Datei), ohne Server, ohne Datenbank.
- Es gibt **keine** Netzwerk-Anfragen (kein fetch/XHR/WebSocket, kein Formular-Versand),
  **kein** localStorage/Cookies und **kein** Tracking oder Analytics.
- Eine Content-Security-Policy im HTML-Kopf **verbietet dem Browser technisch**,
  irgendetwas zu senden (`connect-src 'none'`, `form-action 'none'`).
- Vom Passwort wird **ausschliesslich die Anzahl Zeichen** ausgelesen – die Zeichen
  selbst werden nie gespeichert, angezeigt oder verarbeitet. Alle Felder werden nach
  dem Klick sofort geleert.
- Die eingegebene E-Mail/Telefonnummer wird nur lokal auf dem eigenen Bildschirm
  angezeigt und verschwindet beim Neuladen der Seite.

Der Quellcode in `index.html` ist kurz und kann von allen überprüft werden.

## Marken & Inhalte

«UmfragePortal» ist ein frei erfundener Name. Die Seite verwendet keine Logos oder
Designs echter Firmen, Schulen oder Behörden und gibt sich nicht als solche aus.

## Hinweise für Lehrpersonen

- Bitte vorab darauf hinweisen bzw. im Nachgang klarstellen, dass nichts gespeichert wurde.
- Am besten Schülerinnen und Schüler auffordern, **kein echtes Passwort** einzugeben –
  oder die Demo nutzen, um genau dieses Verhalten zu besprechen.
- Die Seite nur während der Lektion online stellen und danach wieder deaktivieren.
- Nicht für echte Phishing-Angriffe oder ausserhalb des Unterrichts verwenden.

## Dateien

```
index.html      Die komplette Seite (HTML, CSS, JavaScript)
img/logo.png    Logo im Header
img/hero.png    Banner-Bild
img/note.png    Bild der 10er-Note
img/phished.png Foto auf der Aufklärungsseite
```

Fehlt ein Bild, erscheint automatisch ein grauer Platzhalter.
