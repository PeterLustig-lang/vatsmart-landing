# VATSmart Landing Page

Dieses Repository enthält die Quell­dateien für die Landing‑Page und die Pre‑Order‑Bezahlung für VATSmart.

## Deployment auf GitHub Pages

GitHub Pages kann aus dem Root‑Verzeichnis oder aus einem `docs`‑Ordner auf dem `main`‑Branch veröffentlichen【64275134407162†L92-L99】. In diesem Projekt nutzen wir den `docs`‑Ordner als Quelle. Um GitHub Pages zu aktivieren:

1. Wechsle zu den **Repository‑Einstellungen → Pages** (du benötigst Admin‑Rechte).
2. Unter **Source** „Deploy from a branch“ auswählen.
3. Als Branch `main` und als Folder `docs/` einstellen und **Save** klicken【64275134407162†L115-L144】.
4. GitHub baut und veröffentlicht deine Seite. Nach einigen Minuten ist sie unter `https://<username>.github.io/vatsmart-landing/` erreichbar.

Für eine benutzerdefinierte Domain erstelle im `docs`‑Ordner eine Datei namens `CNAME` mit deiner Domain und verweise deinen DNS‑Eintrag auf die GitHub‑Server.

## Stripe Payment Link

Diese Seite nutzt Stripe Payment Links. Payment Links erlauben es dir, Zahlungen ohne Backend zu akzeptieren; du teilst lediglich einen Link und Stripe übernimmt den Checkout‑Prozess【724769404330870†L114-L121】. Nach dem Abschluss einer Checkout‑Session leitet Stripe den Kunden auf deine Success‑URL weiter, wo du weitere Informationen anzeigen kannst【980067080277109†L170-L174】.

Der Test‑Payment‑Link für die Solo‑Lizenz ist bereits im HTML eingebunden:

- Solo‑Lizenz: https://buy.stripe.com/test_dRm8wPcBn4zFfn65jk9AA00

Wenn du Preise änderst oder weitere Pläne erstellst, erstelle neue Payment Links in Stripe und ersetze die Links im HTML.

## Unterstützung

Bei Fragen erreichst du uns unter [support@vatsmart.app](mailto:support@vatsmart.app).
