WERBUNG

# CrowPanel Kalender

ESPHome-Projekt für ein 5,79-Zoll-CrowPanel. Seite 1 zeigt Kalendertermine
aus Node-RED, Seite 2 Temperatur und Luftfeuchtigkeit aus Home Assistant.
Der Drehgeber wechselt zwischen den Seiten.

## Einrichtung

```sh
cp secrets.example.yaml secrets.yaml
# secrets.yaml mit WLAN, API-Key und Kalender-URL ausfüllen
esphome run crowpanel.yaml
```

Die Beispieltermine stehen in `calendar_test.json`. `.esphome/`,
`secrets.yaml` und lokale Build-Dateien gehören nicht ins Repository.
