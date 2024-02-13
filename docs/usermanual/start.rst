Inbetriebnahme
==============

In diesem Abschnitt wird erkl�rt wie eine Erstinbetriebnahme eines OBP60 erfolgt. Die Erstinbetriebnahme kann am einfachsten vorgenommen werden, wenn das Ger�t noch nicht im Boot eingebaut ist. Dazu wird das Ger�t mit Strom versorgt und die ersten Einstellungen vorgenommen. So k�nnen sie die Funktionalit�t testen, bevor sie das Ger�t im Boot einbauen.

Stromversorgung
---------------

Die Stromversorgung des OBP60 erfolgt �ber den Steckverbinder CN2. Beim Zuschalten der Versorgungsspannung schaltet sich das OBP60 automatisch ein. Es gibt keinen gesonderten Ein- oder Ausschaltknopf am Ger�t. Benutzen sie f�r die Stromversorgung die Anschl�sse ``+12V`` und ``GNDS``. Dabei wird ``+12V`` mit dem positiven Pol der Batterie verbunden und ``GNDS`` mit dem negativen Pol. Die beiden Anschl�sse der Stromversorgung sind:

* verpolungssicher
* kurzschlussfest
* �berspannungssicher
* ESD-gesch�tzt

Der zul�ssige Spannungsbereich liegt zwischen 10V...28V. Das OBP60 kann in 12V als auch in 24V Bord-Versorgungsnetzen verwendet werden. Bei Spannungen gr��er 28V wird die interne Sicherung im Ger�t ausgel�st.

.. note::
	Im Ger�t ist eine selbtsr�ckstellende Sicherung verbaut, die bei zu hohem Stromverbrauch die Versorgungsspannung selbst�ndig trennt. Sie k�nnen die Sicherung zur�cksetzen, indem sie die Stromversorgung zum OBP60 trennen und den Grund des �berm��igen Stromverbrauchs beseitigen. Danach warten sie ein paar Minuten und schalten dann die Versorgungsspannung wieder zu.

.. important::
	Die bereitgestellte Stromversorgung des OBP60 sollte im Bordnetz mit einer zus�tzlichen Sicherung von mindestens 5A abgesichert werden. Das erfolgt typischer Weise durch das Board-Panel wor�ber die Stromkreise im Boot zugeschaltet werden k�nnen. So vermeiden sie Br�nde bei aufgescheuerten Versorgungsleitungen im Boot. Die interen Sicherung im OBP60 sch�tzt nur das Ger�t und nicht die Versorgungsleitungen!

Schutzkonzept
-------------

Das OBP60 verf�gt �ber ein mehrstufiges Schutzkonzept. Das soll verhindern, dass sich St�rungen im Versorgungsnetz und auf den Datenleitungen im System ausbreiten. Damit wird sichergestellt, dass das OBP60 trotz St�rungen nicht komplett ausf�llt und in wichtigen Teilen weitesgehend funktionsf�hig bleibt. Um dies zu erreichen, sind die Busssysteme:

* NMEA2000
* NMEA0182
* I2C

vom Bordsnetz isoliert aufgebaut.

.. image:: ../pics/Safety_Concept.png
             :scale: 45%

Abb.: Sicherheitskonzept

Im OBP60 ist dazu eine zus�tzliche Stromversorgung enthalten, die die isolierten Schaltungsteile versorgt. Die zus�tzliche Stromversorgung hat die Ausg�nge ``+5Viso`` und ``GND2``, die am Steckverbinder CN1 und CN2 anliegen. Dar�ber k�nnen auch externe Schaltungen bis 200 mA versorgt werden.

.. warning::
	Verbinden sie die unterschiedlichen Massepotenziale ``GNDS``, ``GND``, ``GND2`` und ``Shield`` niemals miteinander! Dadurch geht die Isolations- und Schutzwirkung verloren. Die Massepotenziale d�rfen nicht gleichberechtigt verwendet werden.
	
.. image:: ../pics/Safe_Areas.png
             :scale: 45%

Abb.: Sicherheitskonzept
	