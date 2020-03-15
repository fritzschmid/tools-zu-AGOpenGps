Liesmichdatei für autosteerFS

die geschwindigkeitsausgabe wird an Pin 12 ausgegeben aub Basis 130 pulse/m

TeilbreitenPort auf 1: die Teilbreiten (ersten 8) werden per Portexpander PCF8574 Adresse hex20 ausgegeben
UturnPort auf 1: die Uturn funktionen werden per Portexpander PCF8574 Adresse hex24 ausgegeben

Master Teilbreite Pin 11 Wenn mindestens eine Teilbreite Aktiv ist auch Pin 11 Aktiv

Beim Rechtseinschlag ist ein Faktor Möglich zb 1.25
	wenn mittig Zerowinkel eingestellt wird und nach Links mit CountsPerDegree der Linkswinkel zb auf 40Grad eingestellt wird,
 	kann sein das Rechts der Winkel ein anderer angezeigt wird - das kann mit dem wert im Sketch angepasst werden.

Overall gain ist in diesem Sketch der Maximale PWMwert dür Lenkmotor es wird dabei mit ProportionalGain alleine das ansprechverhalten eingestellt.
vorher Proportional 25, Overall 20, Min pwm 15
dieser Sketch Proportional=38, Overall 255 wenn keine Strombegrenzung erfolgen soll, Min PWM 15
	der oiginalsketch errechnet (Proportional * (Overall/10) * Lenkwinkeldifferenz) + Minpwm
	beispiel:25*(20/10)*2 +15 =115 währe der Pwm wert
	dieser Sketch(38*1.32*2)+15=115

	

