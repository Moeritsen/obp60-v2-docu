Datenaustausch
==============

Der Datenaustausch im OBP60 kann auf verschiedene Weise erfolgen. Grunds�tzlich stehen mehrere �bertragungsarten �ber verschiedene �bertragungswege zur Verf�gung:

�bertragungsarten
-----------------

* Simplex
	* Daten k�nnen in nur eine Richtung �bertragen werden
* Halbduplex
	* Daten k�nnen abwechselnd, aber nicht gleichzeitig, in beide Richtungen flie�en
* Vollduplex
	* Daten k�nnen in beide Richtungengleichzeitig gleichzeitig �bertragen werden. 
	
�bertragungswege
----------------

* NMEA2000
	* Kabelgebunden NMEA2000-Bus (halbduplex)
	* USB via SeaSmart (vollduplex)
	* �ber WiFi via SeaSmart (vollduplex)
* NMEA0183
	* Kabelgebunden NMEA0183-Bus (simplex)
	* USB (vollduplex)
	* �ber WiFi via TCP (vollduplex)
	* �ber externen Multiplexer (simplex)
* I2C (halbduplex)
* 1Wire (halbduplex)

Datenquellen
------------

Als Datenquellen werden Ger�te bezeichnet, die �berwiegend Daten zur anderen Ger�ten senden und selber nur Daten zur Parametrierung empfangen. Dazu z�hlen folgende Ger�te:

* GPS-Empf�nger (Position, Geschwindigkeit, Richtung)
* Windsensor (Geschwindigkeit, Richtung, Temperatur)
* Tiefen-Sensor (Tiefe, Geschwindigkeit, Wassertemperatur, Entfernung)
* Ruderlage (Winkel)
* Winkelsensoren (Mast, Gro�baum, Foil, Trimmklappen)
* Elektro-Sensor (Spannung, Strom, Leistung, Energie)
* Umgebungssensoren (Lufttemperatur, Fuftdruck, Luftfeuchtigkeit, Helligkeit, Niederschlag, Zustand, Bewegung)
* Durchflusssensoren (K�hlwasserfluss, K�hlwassertemperatur)
* Druck- und Zugsensoren (�ldruck, Achterstag, Vorstag)
* F�llstandsensoren (Level f�r Wasser, Abwasser, Krafstoff)
* Lagesensoren (Roll-, Pitch-, Nick-Winkel, Beschleunigung, Rotation)
* Temperatursensoren (Luft, K�hlwasser, Raum, K�hlschrank, Wasser, Maschinenraum)
* Elektrogeneratoren (Solar, Wind-, Schlepp- Dieselgenerator,
* Radarger�te
* Funkger�te (Position, AIS-Schiffsverkehr, Anrufer, Meldungen, Notrufe)
* Anzeigeger�te (Multifunktionsdisplays, Plotter)

Datensenken
-----------

Datensenken empfangen Informationen und f�hern bestimmte Aktionen aus.

* Ruder-Aktuator (linear, rotatorisch, hydraulisch, elektrisch)
* Relais und Schalter (elektrische Verbraucher wie Ankerwinde, Licht, Positionsleuchten, L�ftung, Heizung, Ladeger�te)
* Anzeigeger�te (Multifunktionsdisplays, Plotter)
* Multimediager�te (Radio, Lautsprecher)

Einige komplexere Ger�te k�nnen sowohl Datenquelle als auch Datensenke sein, wie z.B. Multifunktionsdisplays oder Plotter.

Nachfolgend werden die �bertragungswege n�her beschrieben.

NMEA2000 - Kabelgebunden NMEA2000-Bus
-------------------------------------

Der kabelgebundene NMEA2000-Bus ist der aktuelle Standard in der Bootsvernetzung. �ber ein NMEA2000-Backbone auf CAN-Basis werden verschiedene Ger�te an das Bussystem angeschlossen. Alle Bus-Teilnehmer k�nnen Daten lesen und schreiben. Dabei sind Sensoren Datenlieferanten, die ihre Daten an Displays und Plotter �bertragen.
