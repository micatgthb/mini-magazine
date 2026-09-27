# Mini Magazin

Ein achtseitiges Fotoheft auf einem A4-Bogen. Die Browser-App läuft ohne Backend und verarbeitet Fotos nur auf dem jeweiligen Gerät.

## Eigenes Hosting mit Plesk

Die `index.html` im Hauptordner ist die direkt lauffähige Website. In Plesk für `minimagazin.someswans.de` unter **Git** dieses GitHub-Repository als Remote-Repository verbinden, den Branch `main` wählen und nach `httpdocs` deployen. Die erste Aktualisierung kann mit **Pull Updates** ausgelöst werden. Für künftige Aktualisierungen die von Plesk angezeigte Webhook-URL bei GitHub unter **Settings → Webhooks** für Push-Ereignisse eintragen und in Plesk **Automatic deployment** verwenden.

Die Datei `dist/index.html` enthält denselben Stand für die bisherige ChatGPT-Site. Bei Änderungen beide `index.html`-Dateien zusammen aktualisieren. `.openai/hosting.json` wird nur für diese Site benötigt.

Die App kann auch lokal ohne Internet durch Öffnen der `index.html` verwendet werden. Beim direkten Öffnen einer Datei kann die automatische Browser-Speicherung eingeschränkt sein; die Schaltflächen **Entwurf als Datei sichern** und **Entwurf öffnen** ermöglichen eine portable Sicherung einschließlich der Fotos. Das verlinkte Faltvideo benötigt Internet und wird erst beim Anklicken geladen.
