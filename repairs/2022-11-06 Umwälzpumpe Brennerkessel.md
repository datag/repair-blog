# Umwälzpumpe Brennerkessel defekt

## Ausgangssituation

Brauchwasser und Heizung war am Morgen kalt.

## Analyse

Ein Blick in den Keller zeigte, dass die Glimmlampe Brennerkessel leuchtete. Die Heizungssteuerung gibt also den Impuls zum Heizen. Der Feuerungsautomat des Brenners war nicht auf "Störung". Der Brennerkessel tickte sekündlich, so wie er es bei der Vorwärmzeit (30s) macht. Jedoch ging der Brenner nicht in die Vorspülzeit bzw. das Gebläse lief nicht los.

Der erste Verdacht war, dass die Ölvorwärmung nicht funktioniert. Also entweder der Wärmer oder der Temperatursensor defekt ist. Das Ölgestänge (Ölvorwärmer/Magnetventil/Düse/...) war Anfang 2020 wegen eines defekten Magnetventils durch ein gebrauchtes Gestänge ausgetauscht worden.

Eine kurze Recherche in der Anleitung des Brenners zum Feuerungsautomat (Landis `LOA 36`) zeigte, dass eine temporäre (!) Überbrückung von Anschlussklemme 8 (`OH/L2` - Ölvorwärmer) und 3 (`M` - Motor mit Gebläse) möglich sein sollte, da der Öltemperaturwächter (`OW`) dazwischen sitzt.

![](./assets/2022-11-06%20Feuerungsautomat.png)

Bevor ich das versuchen wollte, galt es nochmals einen Versuch zu starten. Der Brenner sprang sofort und ohne Vorwärmzeit an. Entweder war der Temperatursensor "grob" defekt, oder meine erste Vermutung scheidet aus. Den Überbrückungsversuch verwarf ich damit.

Mir war dann erst aufgefallen, dass die Kesseltemperatur größer-gleich der eingestellten Temperatur war. Der Brenner lief also kurz zuvor. Wieso aber war der Wasserspeicher und die Heizung dann kalt?

Nächste Vermutung war somit die Umwälzpumpe: Entweder die Heizungssteuerung gibt der Pumpe keinen Strom (z.B. defektes Relais), oder aber die Pumpe ist defekt. Ersteres konnte ich durch Messen der Spannung an der Zuleitung zur Pumpe ausschließen - die Pumpe würde also normalerweise in diesem Zustand laufen. Es musste also die Pumpe sein.

![](./assets/2022-11-06%20Umwälzpumpe.jpg)

Leichte Schläge an die Pumpe bewegten sie nicht zum Wiederanlaufen. Vermutung war nun defekter Kondensator (nicht gemessen) oder festgefressene Pumpe.

## Lösung

Glücklicherweise hatte ich noch eine passende gebrauchte Pumpe in Reserve, welche ich dann einbaute. Sie musste nach der längeren Lagerzeit mit ein paar Schlägen zum Anlaufen gebracht werden, läuft nun jedoch einwandfrei.

## TODO

Ersatz für den Anlauf-Kondensator (2,6 µF/ 400 V) ist bestellt und wird in einem Follow-Up in die defekte Pumpe eingebaut.

