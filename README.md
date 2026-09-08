# h2b Humanity System — Website

Statische Website, bereit für GitHub Pages. Jede HTML-Datei ist eigenständig (Bilder, Schriften-Verweise und Skripte eingebettet); nur das Hero-Video liegt separat unter `img/`.

## Dateien

| Datei | Seite |
| --- | --- |
| `index.html` | Startseite (mit Humanity Check) |
| `humanity-system.html` | Das Humanity System (inkl. Für wen?, Warum h2b, FAQ) |
| `ueber-uns.html` | Über uns (inkl. Humanity Audit™) |
| `wissenswertes.html` | Wissenswertes (Whitepaper, Case Studies, Beiträge) |
| `beitrag-*.html` | Die drei Blogbeiträge |
| `kontakt.html` | Kontakt |
| `rechtliches.html` | Impressum, Datenschutz, AGB (Platzhalter) |
| `img/hero-startseite.mp4` | Hero-Video der Startseite |
| `.nojekyll` | Verhindert, dass GitHub Pages die Dateien durch Jekyll verarbeitet |

## Veröffentlichen auf GitHub Pages

1. Auf github.com ein neues Repository anlegen, z. B. `h2b-humanity-system`. Für GitHub Pages im kostenlosen Plan muss es **Public** sein.
2. Alle Dateien und Ordner aus diesem Verzeichnis in das Repository laden — direkt ins Wurzelverzeichnis, `index.html` darf nicht in einem Unterordner liegen. (Web-Oberfläche: „Add file → Upload files"; oder per Git: `git init`, `git add .`, `git commit -m "Website"`, `git branch -M main`, `git remote add origin …`, `git push -u origin main`.)
3. Im Repository: **Settings → Pages**. Unter „Build and deployment" die Quelle **Deploy from a branch** wählen, Branch `main`, Ordner `/ (root)`, speichern.
4. Nach ein bis zwei Minuten ist die Seite erreichbar unter `https://<benutzername>.github.io/<repository>/`.

## Eigene Domain

1. Settings → Pages → **Custom domain**: gewünschte Domain eintragen, z. B. `humanity-system.h2b-kleve.de`.
2. Beim Domain-Anbieter einen **CNAME-Eintrag** anlegen, der auf `<benutzername>.github.io` zeigt (für eine Hauptdomain ohne Subdomain stattdessen die A-Records von GitHub Pages).
3. Sobald der DNS-Eintrag aktiv ist, **Enforce HTTPS** aktivieren.

## Aktualisieren

Geänderte HTML-Dateien einfach im Repository ersetzen (Upload oder Push). GitHub Pages veröffentlicht automatisch neu.

## Was vor dem Livegang noch offen ist

- **Humanity Check und Kontaktformular senden noch nichts.** Die Seite ist statisch; Formulardaten müssen an ein Mail-/CRM-Tool übergeben werden (Formular-Endpunkt eintragen).
- **Terminbuchung**: Platzhalter auf der Kontaktseite, wartet auf den Einbettungslink des Buchungstools.
- **Rechtliches**: Impressum, Datenschutzerklärung (muss den Humanity Check abdecken) und AGB sind Platzhalter.
- **Telefonnummer** auf der Kontaktseite.
- **Inhalte zur Freigabe**: Preismodell (FAQ), Ablauf des Humanity Audit™, Haftungsaussage im Tab „Für Geschäftsführung", Case Studies (Beispielfälle, mit Fußnote gekennzeichnet).
- **Schriftart** wird von Google Fonts geladen. Für eine Datenschutz-saubere Lösung die Schrift Figtree selbst hosten.
