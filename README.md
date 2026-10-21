# Elecrow CrowPanel E-Paper 5.79"
Werbung: www.elecrow.com/crowpanel-esp32-5-79-e-paper-hmi-display-with-272-792-resolution-black-white-color-driven-by-spi-interface.html

Kleine ESPHome-Konfiguration für das CrowPanel-E-Paper mit drei Seiten:

- Begrüßung
- Arch-Linux-Logo
- Temperatur aus Home Assistant

## Einrichtung

1. `secrets.yaml` mit `wifi_ssid` und `wifi_password` befüllen.
2. `archlinux-logo-display.png` im Projektverzeichnis ablegen.
3. Mit ESPHome kompilieren und auf das Board flashen:

```sh
esphome run crowpanel.yaml
```

Die Seiten lassen sich per Wischgeste oder über den Drehgeber wechseln. Die Temperatur kommt aus der Home-Assistant-Entität `input_number.dummy_temperatur`.
