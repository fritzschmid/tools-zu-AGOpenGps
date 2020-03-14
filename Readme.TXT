Abgeänderte Version AgOpenGps_V307
zur Simulationsfahrt über Felder mit Simulierten Gpssiglalen... nicht zur verwendung am Traktor etc

Anpassungen die Ich gut finde:

zusammengeräumter Bildschirm

unter Fahrzeug - Guidance Checkbox damit in der Übersicht AB & Kurven mit Namen angezeigt werden   

unter Fahrzeug - Teilbreite Checkbox Sections:ignoriere Feldgrenze. 
	dabei werden durch Feldgrenzüberschreitungen die Sections bei 
	Automatikfahrt (Workswitch) nicht ausgeschaltet sondern nur bei Überlappen.

Die Strecke Links Unten wird cm genau angezeigt.

Felddaten Links werden mehr Daten angezeigt.

TB Relais (ersten8) und UTurn Relais werden angezeigt.

Menü- Bildschirm - Farben Night/day Modus

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

	Grenzsteine oder Masten Brunnendeckel markiere ich mit Flagge zusätzlich damit diese im Fahrtfenster angezeigt werden.
	
diese Kml kann mit Bounary  Import kml eingelesen werden.

Achtung: immer in einer Runde das Feld Abtasten!
			

