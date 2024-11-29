#  Dieser Ordner ist zur Unterstützung von Buttons und Hintergründen gedacht.


## Powerpoint
  * Diese Ablage wird nicht in Homeassistant hochgeladen, Grund für diesen Ordner ist lediglich die zentrale Ablage von Vorlagen.
  * Vorlage zur Erstellung von Buttons und Hintergründen.
    * button.pptx
      - Ablage der zentral verwendeten Hintergrundbilder


## Fertige Bilder 
  * Fertige Bilder werden in den jeweiligen Themen-Ornder abgelegt unter www/images/
  * z.b.
    - www/images/jahreszeit/frühling.png


**WICHTIG!!!!**
  * Alle Bilder sollten eine klare Bezeichnung haben. Dies vermeidet Datenkonflikte

    - z.b. Flur
      - Ablageort (www/images/wohnung/flur/)
        - flur.png
        - flur_sonos.png
        - flur_steckdose.png
        - flur_steckdose_links.png
        - flur_steckdose_rechts.png
        - flur.schalter.png
        - flur_schalter_licht_decke.png
        - usw.


#### Ausnahme fertige Bilder (Dynamisch)
  * Sollen Bilder dynamisch angezeit werden, also nach Status soll sich das Bild ändern 
  * z.B Wetter ist cloudy (wolkig) oder sunny(sonnig) wäre das Bild immer gleich bei (www/images/wetter/wetter.png)
   
  * Somit wird das Bild je nach Zustand (dynamisch) abgelegt.
    - z.B Wetter ist cloudy (wolkig) oder sunny(sonnig)
    
      - Ablage der Bilder:
        - www/images/wetter/cloudy.png
        - www/images/wetter/sunny.png
  
  * Jetzt kann das System automatisch auf das richtige Bild zugreifen, wenn sich der Wetterstatus ändert.
    - Dies benötigt selbstverständlich dann auch noch einen Sensor, der den Staus prüft.
    
## Bilder verkleinern
  * Es empfiehlt sich die Bilder von der Dateigröße zu verkleiner.
  * Dies ermöglicht ein schnellers Laden und spart Datenspeicher. Somit bleibt das System schön schlank, sauber und schnell.

  * Möglichkeit um Bilder zu verkleinern: https://www.iloveimg.com/compress-image
