Abgeänderte Version AgOpenGpsV4310:
zur Simulationsfahrt über Felder mit Simulierten Gpssiglalen... nicht zur verwendung am Traktor etc

unter Sections Markieren wird erst beim überschreiten der gesamten Teilbreite diese deaktiviert dabei ist beim grenznahen arbeiten immer die teilbreite eingeschalten solange diese nicht das Feld verlässt.

Fahrgassen: diese kann in den optionen eingestellt werden nach startlinie und alle ... fahrten wieder eine Fahrgasse. dabei wird das Feld:"Fahrgasse" Grün wenn aktiv und das 8.Byte Bit 1 in den Maschinendaten geschalten. beim klichen der Schaltfläche Fahrgasse kann diese manuell ein"gelb" manuell aus"violett" oder Automatisch"rot/grün" geschalten werden. wenn in den Optionen bei Wiederholung 0 eingegeben wird ist der Automatikmodus deaktiviert.
im arduino MaschineUSB:
zb im Setup ArduinoLEDausgang(13) für Fahrgassenausgang deklarieren
  pinMode(13, OUTPUT);
  
  und in serialempfang isDataFound..
      hydLift = Serial.read(); // normaler code
    
    //just get the rest of bytes
    if (Serial.read()==1){digitalWrite(13,HIGH);}else{digitalWrite(13,LOW);}   // diese Zeile abändern die Pinnummer des Ports ggf anpassen
    Serial.read();  //normaler code
...



Linien verschieben abgeändert.
Linien grafischDesignen und mit Namen zu speichern.
Auch eine abgefahrene Kurve kann dabei kopiert werden und für eine andere Maschine mit anderer Breite gespeichert und beim ersten einfahren in die kurve muss diese jedoch noch "genullt" werden aber fährt dann gleich die richtige Spur.

ansonsten vom erfinder Perfekt!
*********************************************************************************************************
Gernzeinmessen nur mit V37!

Abgeänderte Version AgOpenGps_V37
zur Simulationsfahrt über Felder mit Simulierten Gpssiglalen... nicht zur verwendung am Traktor etc

Anpassungen die Ich gut finde:

zusammengeräumter Bildschirm

unter Fahrzeug - Guidance Checkbox damit in der Übersicht AB & Kurven mit Namen angezeigt werden  

Grafische AB/Kurve anlegen - ein Name mit Arbeitsbreite beginnend wird Vorgeschlagen 
	dieser Name sollte vor anlegen noch Überarbeitet werden (Breite mit Grenzbereich zB. 420 Nachbarxx)

unter Fahrzeug - Teilbreite Checkbox Sections:ignoriere Feldgrenze. 
	dabei werden durch Feldgrenzüberschreitungen die Sections bei 
	Automatikfahrt (Workswitch) nicht ausgeschaltet sondern nur bei Überlappen.

Die Strecke Links Unten wird cm genau angezeigt.

Felddaten Links werden mehr Daten angezeigt.

TB Relais (ersten8) und UTurn Relais werden angezeigt.

Menü- Bildschirm - Farben Night/day Modus

AB auswählen: Fenster vergrößert und den AnwendeButton GRÜN hinterlegt damit dieser leichter gefunden wird

Empfangssignal -> Dialog erweitert:

Reiter Datenstream: - ist Originalfenster.

für die weiteren Reiter muss eine Maschine mit Arbeitsbreite 2 cm länge 1cm angelegt werden
	und zb als Messpunkt gespeichert werden das in dieser Version möglich ist.

Reiter Punkt Suchen: - Dabei kann ein Koordinatenpunkt mit der Antenne gesucht werden WGS84 oder UTM

Reiter Position: - bei geschlossenem Feld ist das Dateiverzeichnis für die Koordinatendateien 
	im Rootverzeichnis der Felder (Fields)!
	ansonsten im Feldordner.(es Sollte immer das Entsprechende Feld angelegt und geöffnet sein!!!

	[Lösche Positionsdateien] Leert die PositionsTextdateien.
	[Speichere GPS-PositionGanzesFeld] Speichert die Aktuelle Antennenposition in die Datei GPSposition.txt
	[Speichere GPS-Position Option Ohne Brache] Speichert die Aktuelle Antennenposition in die Datei GPSpositionOB.txt
	[Speichere GPS-Position Option NUR Brache] Speichert die Aktuelle Antennenposition in die Datei GPSpositionNB.txt
	[NurPunktSammeln] Speichert die Aktuelle Antennenposition in die Datei GPSpositionNP.txt
	->alle Punkte werden auch in die Datei GPSpositionenAP.txt gespeichert
	[erstelle KML aus GPS Punkten] erstellt 3 KMLdateien aus Ganzes Feld- Nur Brache- und Ohne Brache- -Dateien gleicher Name wie Oben

	werden mehrere Insel in einem Feld nötig diese als NUR BRACHE anlegen - kml erzeugen 
	und dann im Fieldordner diese KML entsprechned umbenennen (Baum1.kml ...) dann die nächste Brachefläche etc.

	Grenzsteine oder Masten Brunnendeckel markiere ich mit Flagge zusätzlich damit diese im Fahrtfenster angezeigt werden.
	
diese Kml kann mit Bounary  Import kml eingelesen werden.

Achtung: immer in einer Runde das Feld Abtasten!
			


