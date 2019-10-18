# toolss-zu-AGOpenGps
zusatztools für AGOpenGps
Hallo AGOpenGps Nutzer!

FieldSectionsLoeschen:
  Zusatztool zum alleinigen archivieren der Sections.txt Datei der in den FieldsOrdner enthaltenen Datei
  Die Originaldatei Sections.txt wird mit neuen Namen des letzten änderns ergänzt.
  eine Leere Datei wird aus Vorlage Sections_leer.txt einkopiert.
  die beiden Dateien Sections_leer.txt und FeldSectionsLoeschen.exe müssen im Ordner Fields befinden, 
  verknüpfung auf Taskleiste wird danach empfolen.

    Programm selber:
    Dir Felder werden in der Liste angezeigt.
    wird ein Feld in der Liste ausgewählt kann mit der Schaltfläche 
    [Sections aus ausgewähltem Feld loeschen] archiviert und    geleert werden.

    Bei [ALLE...] werden Alle Felder"geleert"
viel Erfolg damit

FeldAusVorlage:
  Zusatztool zum Einkopieren von angelegten Felder für AGOpenGPS
  Die Datei FeldAusVorlage.exe muss im Ordner in dem sich der Ordner Fields befindet sein!
  in diesem Ordner muss ebenfalls ein Ordner mit FieldsVorlage mit den darin enthaltenen Feldordner vorhanden sein! 
  verknüpfung auf Taskleiste wird danach empfolen.

    Programm selber:
    Dir Felder werden in der Liste angezeigt.
	    Wenn die Schaltfläche [VorlageFelder Auflisten] geklicht wird, 
		  werden alle Felder der Vorlage (ordner FieldsLorlage) aufgelistet.
	  Wenn die Schaltfläche [VorhandeneFelder Auflisten] geklicht wird, 
		  werden alle Felder aus Ordner (Fields) von AGOpenGPS aufgelistet.

  wird ein Feld in der Liste ausgewählt erscheint dieses Feld im darüberstehenden Textfeld
  hier den Namen ergänzen oder ändern...
  mit der Schaltfläche [Feld aus Auswahl erstellen] 
	  wird das Feld (Ordner) mit allen Dateien der Auswahl 
	  als neues Feld (Ordner) angelegt
	  vorhandene Sections als neue(leere) Datei eingefügt
	  und der Name des Feldes angepasst.
viel Erfolg damit

TextzuKml:
dieses Tool erstellt aus 
Textkoordinaten aus WGS84 koordinaten 
KML Dateien die in Google Earth und 
AGOpenGps als Feld Boundary oder Brachen/Inseln in Felder eingelesen werden können.

!Die Teatdatei kann mit GIS-der AMA Feldstücke erstellt werden!
Feld im Gis anzeigen - Extras - KordinationToolbox. die Feldpunkte in einer Runde anklicken dabei werden kordinaten im Bild angezeigt
ist das Feld fertig markiert in dieser Toolbox mit TXT export wird eine Datei (Ordentlichen Namen Angeben) der Kordinaten erstellt.
Bitte die koordinaten in eine richtung um die Feldgrenze anlegen!

diese Datei kann mit dem Programm gefiltert und als kml ausgegeben werden

die Anwendung mit leer.kml und die erzeugten Textfelddateien im gleichen ordner verwenden.

