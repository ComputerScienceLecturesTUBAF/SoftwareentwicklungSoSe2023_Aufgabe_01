# Softwareentwicklung SoSe2023 - Aufgabe 01

Mit dem Aufgabeblatt werden die in der Vorlesung vorgestellten Basiskonzepte der Programmiersprache C# vertieft.

## Bearbeitungszeit

SWE: 8. Mai - 12. Mai 2023 (Mm, BWM, ROB, BAI, BGIP, BBWL, BBL, MGIN)

Einführung in SWE: 15. Mai - 26. Mai 2023 (KGB, BENG, VTC, MB)


## 1. Datentypen, Ein- und Ausgabe, Auswahl

In einer Parallelwelt bietet eine Telefongesellschaft ihren Kunden den folgenden Mobilfunktarif:

*In der monatlichen Gebühr von 3,99 Euro sind 100 freie Minuten eingeschlossen, darüber hinaus kostet jede Minute 9,9 Cent.*

1. Erstellen Sie ein Programm, das die Monatsgebühr in Abhängigkeit von der Minutenzahl berechnet. Legen Sie die Minutenzahl zunächst testweise im Code fest.

2. Realisieren Sie eine dynamische Eingabe der Minutenzahl z. B. über die Kommandozeile.

3. Für das Datenvolumen stehen drei Tarifoptionen zur Auswahl, die ebenfalls monatlich abgerechnet werden:

    - **Tarif S**: 3 GB Datenvolumen für 5 Euro
    - **Tarif M**: 6 GB Datenvolumen für 7 Euro
    - **Tarif L**: 10 GB Datenvolumen für 10 Euro

    Lesen Sie zusätzlich zur Minutenzahl auch den gewählten Tarif ein (z.B. als `char`) und passen Sie die Berechnung der Monatsgebühr entsprechend an.

## 2. Kontrollfluss

Im Gregorianischen Kalender wird das Schaltjahr wie folgt [definiert](https://de.wikipedia.org/wiki/Schaltjahr#Gregorianischer_Kalender):

 - *"Die durch 4 ganzzahlig teilbaren Jahre sind, abgesehen von den folgenden Ausnahmen, Schaltjahre."*
 - *"Säkularjahre, also die Jahre, die ein Jahrhundert abschließen (z. B. 1800, 1900, 2100 und 2200) sind, abgesehen von der folgenden Ausnahme, keine Schaltjahre."*
 - *"Die durch 400 ganzzahlig teilbaren Säkularjahre, zum Beispiel das Jahr 2000, sind jedoch Schaltjahre."*

1. Bestimmen Sie in einem Programm für ein einzulesendes Jahr, ob es sich um ein Schaltjahr handelt.
2. Ergänzen Sie das Programm um die wiederholte Eingabe des Jahres, bis eine leere Zeichenkette eingegeben wird.
   Verwenden Sie dazu eine `do-while`-Schleife.

## 3. Datentypen, Arithmetik

Berechnen Sie den Funktionswert der Funktion

<a href="https://www.codecogs.com/eqnedit.php?latex=f(x)&space;=&space;\frac{3x&space;-&space;6}{(x&space;&plus;&space;2)(x&space;-&space;1)^2}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?f(x)&space;=&space;\frac{3x&space;-&space;6}{(x&space;&plus;&space;2)(x&space;-&space;1)^2}" title="f(x) = \frac{3x - 6}{(x + 2)(x - 1)^2}" /></a>

im Intervall `[a, e]` mit der Schrittweite `s`.
Die Intervallgrenzen sowie die Schrittweite sind einzulesen, x- und y-Werte sind tabellarisch auszugeben.
Es soll möglich sein, reelle Zahlen als Schrittweite anzugeben.

*Hinweis: Beachten Sie die Polstellen der Funktion und die Besonderheiten des Vergleichs von `double`-Werten.*

## 4. Wiederholung, Array

Die böse Stiefmutter hat Wal-und Haselnüsse miteinander vermischt.
Das Aschenbrödel muss die Nüsse wieder trennen und dabei die Anzahl und das durchschnittliche Volumen pro Sorte ermitteln.
Die Gesamtzahl der Nüsse ist leider unbekannt, aber zwei Hinweise hat sie von der Stiefmutter bekommen:

 - Alle Nüsse mit einem Durchmesser kleiner als 2cm sind Haselnüsse, alle anderen sind Walnüsse.
 - Das Volumen einer Nuss ist bestimmbar durch: <img src="https://render.githubusercontent.com/render/math?math=V = \frac{1}{6} \pi d^3">.

1. Schreiben Sie ein Programm, das ein Array mit zufälliger Länge und zufälligen Werten zwischen 0.75 und 4 initialisiert.
   Es repräsentiert die Durchmesser der Nüsse.
2. Ergänzen Sie das Programm um eine Funktion, die dem Aschenbrödel hilft, indem sie die Anzahl sowie das durchschnittliche Volumen von Wal- und Haselnüssen bestimmt.

## 5. Wiederholung

Es soll folgendes Spiel durch ein Programm simuliert werden:

Der Spieler zahlt für jedes Spiel einen Einsatz von 1 Euro.
Er darf einmal mit 3 Würfeln würfeln.
Je nach gewürfelter Punktzahl bekommt der Spieler einen Gewinn entsprechend der folgenden Tabelle ausgezahlt:

Punktzahl | Gewinn in EUR
---       | ---
3-15      | 0
16        | 5
17        | 10
18        | 100

Simulieren Sie 1000 Spiele mit zufälligen Würfen und geben Sie die zugehörige Gewinn- Und Verlustrechnung inkl. Bilanz aus.

## 6. Array

CO2-Ausstoß zweier Inselstaate, karibischer „St. Kitts und Nevis“ und pazifischer „Niue“ in den letzten 10 Jahre soll in einem Programm vergleichend betrachtet werden.

Erstellen Sie dazu zwei Arrays und Initialisieren Sie diese mit Werten. Vergleichen Sie die Werte paarweise miteinander und geben sie die Meldung aus, welcher der Staaten den größeren Ausstoß im jeweiligen Jahr hatte.
Zu bestimmen ist weiterhin, welcher der Staaten den größten jährlichen Ausstoß hatte, betrachtet über alle Jahre.

## 7. Array

Schreiben Sie ein Programm, das die Namen der 10 Erstplatzierten (s. Tabelle) eines Weltcups in einem Array speichert. Geben Sie die Daten mit Hilfe einer foreach-Anweisung als Markdowntabelle aus. Anschließend soll wiederholt ein Index eingegeben werden und der Name des entsprechenden Rangierten ausgegeben werden. Berücksichtigen Sie dabei mögliche *Format-* und *IndexOutOfRange-* Ausnahmen.

Platzierung | Name
---- | ---------------------------
1	 | Marte Olsbu Röiseland
2	 | Elvira Öberg
3	 | Lisa Theresa Hauser 
4	 | Hanna Öberg
5	 | Anais Chevalier-Bouchet
6	 | Denise Herrmann 
7	 | Dzinara Alimbekava
8	 | Justine Braisaz-Bouchet
9	 | Dorothea Wierer
10 | Marketa Davidova


**Wir sind auf Ihre Lösungen gespannt!**
