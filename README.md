# NutriPlan – iPhone-Web-App (PWA)

## Inhalt
- `index.html`: App-Oberfläche, Rezeptverwaltung und lokale Speicherung
- `manifest.webmanifest`: Installationsinformationen
- `sw.js`: Offline-Cache (Service Worker)
- `icons/`: App-Symbole

## Auf dem iPhone installieren
1. Lade den gesamten Ordner auf einen Webhoster hoch, der HTTPS unterstützt (z. B. eine eigene Website oder einen statischen Hosting-Dienst).
2. Öffne die HTTPS-Adresse in Safari auf dem iPhone.
3. Tippe auf „Teilen“ → „Zum Home-Bildschirm“ → „Hinzufügen“.
4. Öffne NutriPlan über das neue Symbol. Lade die App einmal mit Internetverbindung vollständig, damit der Offline-Cache eingerichtet wird.
5. Danach kann die App-Oberfläche auch ohne Internet geöffnet werden.

Wichtig: Service Worker und PWA-Installation benötigen HTTPS (außer auf localhost). Die Dateien allein werden nicht automatisch auf deinem iPhone installiert.

## Speicherung & Datenschutz
Rezepte, Favoriten und die Tagesauswahl werden mit `localStorage` lokal im Browser auf diesem Gerät gespeichert. Es gibt keine Anmeldung und keinen Server, der deine Rezeptdaten erhält. Browserdaten löschen oder Safari-Daten zurücksetzen kann diese Daten entfernen. Export/Cloud-Backup ist in dieser ersten Version noch nicht eingebaut.

## Hinweis zu Kalorien
1.900 kcal ist das von dir vorgegebene Tageslimit. Die App bewertet nicht, ob dieses Limit für deine Ziele und deinen individuellen Bedarf passend ist. Nährwerte der Beispielrezepte sind Schätzwerte und sollten bei Bedarf anhand konkreter Zutaten und Mengen angepasst werden.
