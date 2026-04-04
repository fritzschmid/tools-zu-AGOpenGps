AgOpenGps Vermessungstool
basis ist agopengps V6 in der ein zusatztool unter werkzeug Messspunkte erstellt wurde.

Als Arbeitsgerät zum Suchen von Grenzsteinen und Linien sollte ein 100cm breites Gerät angelegt werden!!!

das"Fahrzeug" ist ein kleiner Blauer Antennenpunkt mit einer Einrahmung punkt zu aussen 1m
Das Feld ist in dieser Version richtung Norden ausgerichtet um bei suchen von Punkten mit der Antenne nicht das Feld im Bild dreht.

in diesem können externe Koordinaten aus dateien wie Kml, Xml, Json, Txt in Textdateien ungewandelt und diese dann importiert werden.
diese importierten Dateizeilen können als Feldgrenze, Suchkoordinaten Hilfslinien, grenzsteinsuche etc herangezogen werden.
aus den fertigen Datenzeilen kann dann eine KML erstellt und diese dann als Grenze importiert werden. 
Auch späteres verändern von Punkten und dabei die Neue Feldgrenze automatisch ersetllen ist dann möglich.

Koordinateneigabe mit Umrechnung zum Suchen und Anlegen von Punkten aus:
WebMercator; UTM32N; UTM33N; MGI GK M34,M31,M28 ;BMN M34,M31,M28 
zb. aus Kataster.gv.at moglich aber umrechnung mur für Hobbyanwendung und nicht für Grenzstreit! das muss ein Geometer dann richtigstellen.

Wird eine Spur einschaltet ist die Ausrichtung dann der Spur entlang! Dabei wird die Spurabweichung in[m] und cm angezeigt wenn das Gerät 100cm Arbeitsbreite hat.

IsoXml Taskdata wird mit Feldnamen im unterordner v4 abgelegt um besser auf andere terminals verwendbar und unverwechselbarer ist (Hausacker_TASKDATA.xml)

weitere Änderungen zur Normalversion von BT
Anlegen von Fahrgassen anders
anlegen von Curven aus RecPath damit diese dann beliebig begonnen und in beiden Richtungen verwendet werden können- mit meiner Version dann auch ohne weiterspiegeln befahrbar da Spurnamen mit $ 
Couturspuren anlegen aus ABs zb bei Konische Felder kann damit von den ABs der beiden aussenliegenden Spuren aufbefächert countuspuren angelegt werden und diesen auch nachgefahren werden.

Felddaten dann für Normalversion V6 verwendbar!
