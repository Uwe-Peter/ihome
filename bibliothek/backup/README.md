# Home Assistant Konfiguration

Dies ist meine private [Home Assistant](https://home-assistant.io/) Konfiguration. Diese Instanz läuft auf einem Raspberry Pi 4 [nach dieser Anleitung](https://home-assistant.io/docs/installation/raspberry-pi/).
Zu jedem Verzeichnis gibt es eine kurze Readme-Datei, in der erklärt wird, was sich darin befindet und welchen Zweck die einzelnen Dateien oder Dateigruppen erfüllen.


## Installation Addo-on (mit HA) in Backup Reset enthalten
  [File editor](https://github.com/home-assistant/addons/tree/master/configurator)
  * Mit dem File editor wird der Zugriff auf die Strucktur von Homeassistant ermöglicht. Zwingend erforderlich.
    - Beim Booten starten -on
    - Watchdog -on
    - Automatische Updates -on
    - In der Seitenleiste anzeigen -on
    - Starten
    - Warten bis File editor gestartet ist und System neu starten
        
  [Terminal & SSH](https://github.com/hassio-addons/addon-ssh)
  * Mit dem Terminal & SSH wird der Zugriff auf SSH von Homeassistant ermöglicht. Zwingend erforderlich.
    - Passord vergeben
      - z.b.
        - username: **user**
        - password: **123456**
      - Beim Booten starten -on
      - Watchdog -on
      - Automatische Updates -on
      - In der Seitenleiste anzeigen -on
      - Starten
      - Warten bis Terminal & SSH gestartet ist und System neu starten
  
  [HACS](https://hacs.netlify.com)
  * Zum Installieren, Aktualisieren und Auffinden neuer benutzerdefinierter Integrationen. Alle anderen benutzerdefinierten Integrationen werden über dieses Programm installiert.
    - Terminal & SSH aus der Seitenleiste öffnen
    - Code in Befehlszeile eingeben
      - **wget -O - https://get.hacs.xyz | bash -**
      - bestätigen und durchlaufen lassen
    - System neu starten
    - Strg + F5 (cach leeren)
    - Jetzt ist HACS in Geräte & Dienste als integration zu suchen und zu installieren
    - HACS aus der Seitenleiste öffnen
      - HACS verbindung mit Github herstellen (Code in Github eingeben, erfordert ein Github-Konto (privat reicht aus, ohne Einträge)
        - Zugriff in Github bestätigen und wieder zurück zu HACS
        - HACS einen Bereich(Räume) zuweisen und bestätigen.
          - **20 min warten und System neu starten**
        - Jetzt ist HACS verfügbar und kann genutzt werden


## Erstellung Bereiche Bereiche & Zonen (mit HA) in Backup 2. Reset enthalten
  * Bereiche werden benötigt um Geräte und Dienste einzelnen Räumen zuzuordnen.

    - z.B -Küche
    - Wohnzimmer
    - Schlafzimmer
    - Kontrollraum (Technik die keinen Räumen zugeordnet werden sollen)
    - usw.


## Die von mir verwendeten Geräte, Dienste und Software (mit HA)
  * Sonos [SONOS](https://www.home-assistant.io/integrations/sonos)
    - Mit der Sonos-Integration können Sie Ihre drahtlosen Sonos-Lautsprecher steuern. Sie funktioniert auch mit IKEA Symfonisk-Lautsprechern.
  * Mond [Moon](https://www.home-assistant.io/integrations/moon)
    - Die Mond-Integration verfolgt die Phasen des Mondes.
  * Sternzeichen [Zodiac](https://www.home-assistant.io/integrations/zodiac)
    - Die Zodiac-Integration verfolgt das aktuelle Tierkreiszeichen.
  * Sonne [Sun](https://www.home-assistant.io/integrations/sun)
    - Die Sonnenintegration verwendet den in der Home Assistant-Konfiguration eingestellten Standort, um festzustellen, ob die Sonne über oder unter dem Horizont steht.
  * Kalender [Holyday](https://www.home-assistant.io/integrations/holiday)
    - Mit der Feiertagsintegration können Sie einen Feiertagskalender in Home Assistant erstellen, um Automatisierungen zu steuern.
  * Camera [Generic Camera](https://www.home-assistant.io/integrations/generic)
    - Mit der generischen Kameraplattform können Sie eine beliebige IP-Kamera oder eine andere URL in den Home Assistant integrieren.
  * Bluetooth [Bluetoot](https://www.home-assistant.io/integrations/bluetooth)
    - Die Bluetooth-Integration erkennt Bluetooth-Geräte in der Nähe. Erkannte Geräte werden im Abschnitt "Erkannte" auf der Seite "Integrationen" im Konfigurationsbereich angezeigt.
  * Wetter [Meteorologisk institut](https://www.home-assistant.io/integrations/met)
    - Die Met-Plattform nutzt den Webdienst Met.no als Quelle für meteorologische Daten für Ihren Standort.
  * Wetterwarnung [DWD Weather Warnings](https://www.home-assistant.io/integrations/dwd_weather_warnings)
    - Die Integration der Wetterwarnungen dient als Quelle für aktuelle und vorausschauende Wetterwarnungen.
  * HACS [HACS](https://hacs.netlify.com) in Backup Reset enthalten
    - Erfordert zuerst die Installation von HACS
  * Pollenflug [DWD Pollenflug](https://github.com/mampfes/hacs_dwd_pollenflug) 
    - Erfordert zuerst die Installation über HACS  
  * Mobile App [Mobile App](https://www.home-assistant.io/integrations/mobile_app)
    - Die Mobile App-Integration ermöglicht die einfache Integration von Home Assistant-Mobilanwendungen in Home Assistant.
  * Shelly [Shelly](https://www.home-assistant.io/integrations/shelly)
    - Integrieren Sie Shelly-Geräte in den Home Assistant.
  * Radio [Radio Browser](https://www.home-assistant.io/integrations/radio_browser)
    - Die Integration des Radio-Browsers ermöglicht es Ihnen, das im Radio-Browser gesammelte Verzeichnis von Radiosendern im Home Assistant zu verwenden.
  * IKEA [IKEA TRÅDFRI](https://www.home-assistant.io/integrations/tradfri)
    - Die IKEA TRÅDFRI Integration ermöglicht es Ihnen, Ihr IKEA Trådfri Gateway mit Home Assistant zu verbinden.
  * FITZ Box Smarthome [AVM FRITZ!SmartHome](https://www.home-assistant.io/integrations/fritzbox)
    - Mit der AVM FRITZ!SmartHome Integration für Home Assistant können Sie FRITZ!DECT-Geräte wie Schalter, Sensoren und Thermostate einbinden.
  * HomePod [Apple TV](https://www.home-assistant.io/integrations/apple_tv)
    - Die Apple TV-Integration ermöglicht Ihnen die Steuerung eines Apple TV (jeder Generation).
 
  
## Benutzerdefinierte Integrationen in Backup 1. Reset enthalten
  [HACS](https://hacs.netlify.com) zum Installieren, Aktualisieren und Auffinden neuer benutzerdefinierter Integrationen. Alle anderen benutzerdefinierten Integrationen werden über dieses Programm installiert.
  
  #### (Alle angegebenen Integrationen müssen noch unter Dashboard einzeln aktiviert verden.)
       
  * [default_config_disabler](https://github.com/tronikos/default_config_disabler) ist in Backup (Reset) enthalten.
  * [Simple Thermostat](https://github.com/nervetattoo/simple-thermostat) einfache Darstellung und Bedienung von Thermostaten.
  * [card-mod](https://github.com/thomasloven/lovelace-card-mod) ermöglicht die Anwendung von CSS-Stilen auf verschiedene Elemente des Home Assistant-Frontends.
  * [kiosk-mode](https://github.com/maykar/kiosk-mode) blendet die Kopfzeile und/oder die Seitenleiste im Home Assistant aus.
  * [Mini Media Player](https://github.com/kalkih/mini-media-player) eine minimalistische und dennoch anpassbare Media-Player-Karte für den Home Assistant.
  * [button-card](https://github.com/custom-cards/button-card) Button-Karte für Ihre entities.
  * [Sonos Card](https://github.com/punxaphil/custom-sonos-card) Media-Player-Card für Sonos-Lautsprecher.
  * [auto-entities](https://github.com/thomasloven/lovelace-auto-entities) automatisches aus und einblenden von Entitäten, die bestimmten Kriterien entsprechen.
  * [multiple-entity-row](https://github.com/benct/lovelace-multiple-entity-row) anzeige mehrerer Entitätszustände, Attribute und Icons auf einer Zeile.
    - **HINWEIS: Dies ist keine eigenständige Karte, sondern ein Zeilenelement für die Entitätenkarte.**  
  * [slider-entity-row](https://github.com/thomasloven/lovelace-slider-entity-row) hinzufügen eines Schiebereglers zu einer Zeile.
  * [hui-element](https://github.com/thomasloven/lovelace-hui-element)
  * [Custom brand icons](https://github.com/elax46/custom-brand-icons)
  * [fold-entity-row](https://github.com/thomasloven/lovelace-fold-entity-row) Zeilen einklappen und verstecken in der Karte.
  * [flipdown-timer-card](https://github.com/pmongloid/flipdown-timer-card) Karte für Timer.
  * [Dwd Pollenflug](integration) (https://github.com/mampfes/hacs_dwd_pollenflug) Pollenflugvorhersagen des Deutschen Wetterdienstes (DWD).
  * [Caule Themes Pack 1 - by caule.studio](https://github.com/orickcorreia/caule-themes-pack-1) 
  * [iOS Themes - Dark Mode and Light Mode](https://github.com/basnijholt/lovelace-ios-themes) Eine verallgemeinerte Version des iOS Dark Mode Theme!
    

  ### Benutzerdefinierte Repositorie
  * Hacs
    - Frontend
      - 3 Punkte Menü
      - Benutzerdefinierte Repositorie
 
  #### Repositorie in Backup Reset enthalten        
  * Link eintragen: https://github.com/tronikos/default_config_disabler
    * Kategorie „Integration“
      - zurück zu HACS
        - default_config_disabler auswählen und herunterladen
      - zurück zu Geräte & Dienste
          - Integrationen hinzufügen
            - default_config_disabler suchen und installieren
          - Konfiguration
            - auswählen welche Dienste nicht automatisch geladen werden sollen

  **WICHTIG!!!!!**
  * Nach einem Update von Homeassistant sofort den Rasperry komplett neu Starten, sonst ist dieser Dienst deaktiviert.
  * Automatische aktivierung nach einem Neustart des Raspberry
  
  #### Repositorie in Backup 1. Reset enthalten        
  * Link eintragen: https://github.com/ottes/lovelace-dwd-pollenprognose-card-ottes.git
  * Kategorie „Lovelace“
    - Zurück zu HACS
    - lovelace-dwd-pollenprognose-card-ottes auswählen und herunterladen

 #### Repositorie bei Bedarf installieren 
  * Link eintragen: https://github.com/rbogdanov/lovelace-animated-background.git
  * Kategorie „Lovelace“
    - Zurück zu HACS
    - Lovelace Animated Background updated by rbogdanov auswählen und herunterladen


# Nützliche Links
* [Home Assistant Dokumentation](https://home-assistant.io/docs/) und [Integrationsliste](https://home-assistant.io/integrations/)
