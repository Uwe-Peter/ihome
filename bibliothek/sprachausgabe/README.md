#  Dieser Ordner ist zur Unterstützung von Sprachausgaben, hierfür werden Zusatzinformationen benötigt.


## Sprachausgabe
  * Für die Sprachausgabe ist es notwendig, dass mp3 Dateien vorliegen, die abgespielt werden können, wenn eine Aktion eintritt.
  * Hierfür müssen diese mp3 Dateien erzeugt werden mit dem entsprechenden Inhalt, das diese in einer Automation verwendet werden kann.
    - z.b.
      - Man verlässt die Wohnung und das System prüft ob alles zu ist.
      - Die Fenster im Flur sind noch auf !
          
      - Sprachausgabe von SONOS

        - **Die Fenster im Flur sind noch offen!**
        - Datei: homeassistant/www/mp3/flur/flur_fenster_offen.mp3
  
####  Sprachausgabe .mp3 erstellen und ablegen
  * Die erstellten .mp3 werden im Ordner www und dann im Ordner mp3 abgelegt.
    - wenn dieser Ordner noch nicht vorhanden ist muss dieser angelegt werden.
      - Es empfiehlt sich diese mp3 nach Gruppen zu sortieren und sauber zu bezeichnen.
        - z.b
        - homeassistant/www/mp3/sonos/flur/flur_fenster_offen.mp3

#### Anzulegende Ordner
    - www
      - mp3
        - sonos
          - timer

  * Internetadresse zum erstellen von Sprachnachrichten: [Sprachnachrichten erstellen](https://ttsmp3.com/)    


**WICHTIG!!!!**
  * Der Download ist für den Tag begrenzt.
  * Nach der Texteigabe, bitte die (Read) testen vor dem Download.

    * Durch das setzen von "," wird die Sprache angepasst.
      - Textbeispiel          
        - Die Fenster im Flur sind noch offen!!
      - Download .mp3
      - Umbenennen der .mp3 in: **flur_fenster_offen.mp3**
