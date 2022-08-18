# 02_Decision_Tree

 Binder Badge zum starten des Jupyter Notebooks (Decision_Trees_und_Random_Forests_Projekt_Musterloesung.ipynb) via myBinder:  

In der Umgebung von mybinder können Sie das Übungsbeispiel ausführen lassen, eigene Lösungen codieren (bestehenden Code modifizieren), um das Übungsbeispiel mit dem erwartenden Ergebnis zu reproduzieren.

## Dokumentation zur Übungsaufgabe: 
Aufgebaut ist die Übungsaufgabe in jeweils in Beschreibungsabschnitt was explizit gemacht werden soll. Die jeweilige darunterliegende Zelle stellt den Code Bereich dar, in der dieser Aufgabenabschnitt codiert wird und ggf. den dazugehörigen Output nach der Ausführung (SHIFT + Enter) der jeweiligen Codezelle darstellt.

! Um das zu erwartendee Ergebnis (Output) der Lösung im Übungsbeispiel nicht zu verlieren bzw. zu überschreiben, können Sie nach der Beschreibung der jeweiligen Teil-Aufgabe eine Zwischenzeile(neue Zeile) einfügen, in der Sie Ihre Lösung codieren um danach Ihren Code mit dem darunter liegenden Mustercode + dessen Output vergleichen/überprüfen zu können. 

**Vorgehensweise im Übungsbeispiel:**

Fallbeispiel: In diesem Projekt werden wir mit Fake-Daten zu Werbung arbeiten, die aufzeigen, ob ein Nutzer auf eine Werbeanzeige auf einer Webseite einer Firma geklickt hat oder nicht. Wir werden versuchen ein Modell zu erstellen, das anhand von Nutzereigenschaften vorhersagt, ob dieser auf die Werbung klicken wird oder nicht.

**1. Librarries**
* notwendige Libraries müssen importiert werden (pandas, numpy, matplotlib.pyplot, seaborn) für die Datenverarbeitung und Datenvisualisierung

**2. Rohdaten**
* Rohdaten(advertising.csv) einlesen und DataFrame erstellen
* Deskriptive Statistiken anzeigen und analysieren mit der info() und describe() Funktion

**3. Explorative Datenanalyse**

mittels Plots aus der Seaborn Library können die Daten visualisiert werden, um sie besser analysieren zu können. 
* Histogramm der Spalte "Age" der Daten erstellen
* Jointplot, welches "Area Income" mit "Age" vergleicht
* Jointplot, das die KDE Verteilung von "Daily Time Spent on Site" gegen "Age" aufzeichnet
* Jointplot für "Daily Time Spent On Site" gegen "Daily Internet Usage"
* Pairplot mit "Clicked on Ad" als Hue

**4. Logistische Regression**
* Aufteilen der Daten in Trainings- und Testdaten
* Import der LogisticRegression von sklearn.linear_model 
* Trainiere und fitte ein logistisches Regressionsmodell auf das Trainingsset mit der fit() Funktion

**5. Vorhersagen und Auswertung (erwartendes Ergebnis/Output)**
* Vorhersage der Werte für die Trainingsdaten mit der predict() Funktion, welches auf das zuvor erstellte Regressionsmodell angewendet wird
* Klassifizierungsreport für das Modell, um die Perfomance in Bezug auf Precision und Recall Werte zu erhalten 
