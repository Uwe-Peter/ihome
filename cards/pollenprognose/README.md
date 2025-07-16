[![hacs_badge](https://img.shields.io/badge/HACS-Custom-41BDF5.svg)](https://github.com/hacs/integration)

# pollenprognose-card-ottes

Ein Fork der großartigen Arbeit von [leahoswald](https://github.com/leahoswald/) an einer Karte, jedoch nicht mit HACS nutzbar. Hier ist die Custom Card, die du verwenden kannst.

## Ursprung

Eine Lovelace Custom Card für https://github.com/mampfes/hacs_dwd_pollenflug in Home Assistant, basierend auf der großartigen Arbeit von https://github.com/isabellaalstrom/, https://github.com/isabellaalstrom/lovelace-pollenprognos-card und https://github.com/TekniskSupport.

## Installation

Noch nicht verfügbar, vielleicht in Zukunft: Der einfachste Weg zur Installation ist über HACS (Home Assistant Community Store). Suche im Frontend-Bereich nach **Pollenprognose Card Ottes** und installiere sie (oder einen anderen Fork?).

Für FOW: Installiere dieses Repository als Custom Repo und suche im Frontend nach **Pollen**.

Wenn du **KEIN HACS** nutzt, kannst du die Datei `-ottes.js` plus den Ordner `images` herunterladen und im Verzeichnis  
`homeassistant_config_dir/www/community/lovelace-dwd-pollenprognose-card-ottes/` ablegen.

## Beispielhafte Nutzung  
Wähle die Allergene, die du anzeigen möchtest.

Für den UI-Modus:
```yaml
type: custom:pollenprognose-card-ottes
region_desc: Nordhessen und hess. Mittelgebirge
region_id: 91
allergens:
  - Birke
  - Erle
  - Hasel
  - Esche
  - Graeser
  - Roggen
  - Beifuss
  - Ambrosia
```

Für den YAML-Modus:
```yaml
- type: custom:pollenprognose-card-ottes
  region_desc: Oberrhein und unteres Neckartal
  region_id: 111
  allergens:
    - Birke
    - Erle
    - Hasel
    - Esche
    - Graeser
    - Roggen
    - Beifuss
    - Ambrosia
```

## Optionen

| Name | Type | Standard | Beschreibung
| ---- | ---- | ------- | -----------
| type | string | **Erforderlich** | `custom:pollenprognose-card-ottes`
| region_desc | string | **Erforderlich** | Name der Region, wird nur in der Kopfzeile angezeigt.
| region_id | string | **Erforderlich** | Die Regions-ID, wie vom [defined by DWD](https://opendata.dwd.de/climate_environment/health/alerts/Beschreibung_pollen_s31fg.pdf)  (Name aus der DWD-Komponente suchen und ID hier eintragen).
| allergens | list | **Erforderlich** | Liste der Allergene, für die du Sensoren hast, definiert bei [hacs_dwd_pollenflug](https://github.com/mampfes/hacs_dwd_pollenflug)
| title | boolean | **Optional** | Auf `false` setzen, um die Überschrift der Karte zu entfernen.
| show_state | boolean | **Optional** | Auf `false`e setzen, wenn der Status-Text unter den Bildern nicht angezeigt werden soll.
| forecast | boolean | **Optional** | Auf `true` setzen, um die Prognose für morgen mit einem kleineren zusätzlichen Blatt anzuzeigen.
| filter_unknown | boolean | **Optional** | Auf `true` setzen, um nur aktuell aktive Pollen anzuzeigen.

### Beispiel der Karte mit allen Allergenen dargestellt
![Screenshot2022-02-13_17-16-48](https://user-images.githubusercontent.com/1292551/153762269-214888ae-d2bb-445b-a90a-f4336cd303e1.png)
