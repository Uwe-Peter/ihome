# Dieser Ordner ist zur Unterstützung von Integrationen die Zusatzinformationen benötigen.  


## DWD Warnmeldungen
  * DWD Wetterwarung benötigt den Ort der Warnmeldungen als eine Warnzell-ID
    - Die Datei (cap_warncellids_csv.csv) beinhaltet die Warzellen-ID des Deutschen Wetterdienst.
    - Einfach den Ort aussuchen und die Warnzellen-ID in die Integration eintragen
      - z.b.
        - Warnzell-ID Stadt:
        - **806431013**   (Stadt Lampertheim)

#### Warnmeldungen aktuelles Bild einfügen
  * DWD Wetterwarung kann zusätzlich eine aktuelle Grafik zu Warnemeldung ausgeben.
    - Alle verfügbaren Bilder findet man auf [Warnmeldungen](https://www.dwd.de/DE/wetter/warnungen_aktuell/objekt_einbindung/objekteinbindung.html)
    - Diese werden alle 15 min aktualisiert.
        
      - Hessen, Rheinland-Pfalz, Saarland:
        https://www.dwd.de/DWD/warnungen/warnstatus/SchilderOF.jpg
      - Baden-Württemberg:
        https://www.dwd.de/DWD/warnungen/warnstatus/SchilderSU.jpg

      
**WICHTIG!!!**
  * Hierzu wird die Integration z.b. (Generic Camera) benötigt
