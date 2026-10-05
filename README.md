# bgmon-website

Statische Landingpage für [bgmon](https://github.com/mcfetz/bgmon) — das selbstgehostete
CGM-Monitoring mit Alarmen, AGP-Bericht und BG-Prognose.

Veröffentlicht über GitHub Pages:
**<https://mcfetz.github.io/bgmon-website/>**

## Aufbau

| Datei | Zweck |
|---|---|
| `index.html` | Einzige Seite, deutsch, semantisches Markup |
| `assets/style.css` | Layout und Design, hell und ruhig |
| `assets/logo.svg` | Logo und Favicon |
| `assets/shots/` | Screenshots der bgmon-Oberfläche |

Keine externen Ressourcen: keine CDN, keine Webfonts, kein Tracking. Die Seite lädt
außerhalb der eigenen Domain nichts nach.

## Screenshots

Die Bilder in `assets/shots/` stammen aus der bgmon-Oberfläche mit **synthetischen
Demo-Daten** aus einer separaten Datenbank (`bgmon_demo`). Es sind keine echten
Patientendaten enthalten. Sie werden bei Bedarf neu erzeugt und ersetzt.

## Lokal ansehen

```bash
python3 -m http.server 8080
# http://localhost:8080
```

## Veröffentlichen

Der Build ist der Repository-Inhalt selbst — es gibt keinen Build-Schritt. Nach einem
Push auf `main` veröffentlicht GitHub Pages die Seite neu.

## Lizenz

MIT — siehe [LICENSE](LICENSE).