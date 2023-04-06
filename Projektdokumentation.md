# Projekt-Dokumentation



Daisy: Ben Müller,John Broder, Brandon Spaqi, Christian Aeschlimann

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 23.02.2023| 0.0.1   | Heute haben wir uns unser Thema Pizza runner erfunden und einige Ideen darüber gesammelt, auserdem haben wir mit den User-Stories angefangen und das Pap gemacht.
|02.03.2023| 0.0.2     |Heute haben wir die Planung beendet und haben das Use Case Diagramm überarbeitet.|
|09.03.2023|0.0.3| Heute haben wir uns mit unity vertraut gemcht und mehrere Arbeitspakete angefangen aber keins beendet da es immer wieder grosse Probleme mit Unity gab.|
|19.03.2023|0.0.4|Heute haben wir da weiter gemacht wo wir letztes Mal wegen der Fehler aufhören mussten. Ein Teil unserer Gruppe hat einen ersten Prototypen erstellt, während der andere Teil versuchte die alten Fehler zu beheben, oder versuchte z.B. eine Map in unseren Prototypen zu laden.|
## 1 Informieren

### 1.1 Ihr Projekt

In diesem Programmierprojekt programmieren wir einen Endless-Runner, bei dem man eine Pizza belegt, in dem man die richtigen Zutaten einsammelt. 

Wir wollen mithilfe von Unity einen Endless-Runner programmieren, bei dem man verschiedenen Hindernissen ausweichen muss und gleichzeitig eine Pizza macht, in dem man verschiedene Zutaten einsammeln muss. Wenn eine Pizza fertig belegt ist, bekommt man einen Pizzapunkt und fängt wieder mit einer neuen Pizza an. Während man rennt, fallen in regelmässigen Abständen Pizzaschaufeln vom Himmel, denen man dann ausweichen muss. Neben der exponentiell steigenden Geschwindigkeit des Users, erhöht sich auch die Geschwindigkeit, in dem die Schaufeln vom Himmel fallen. Falls der User eine Zutat zum zweiten Mal einsammelt, wird er «bestraft». Wir haben uns final für 3 Schwierigkeitsmodi entschieden. 


### 1.2 User Stories
| US-№ | Verbindlichkeit | Typ  | Beschreibung                      |
| ---- | --------------- | ---- | ---------------------------------- |
|   1  |Muss             |F     | Als ein Benutzer möchte ich, dass man endlos rennen kann, damit ich Spass habe. | 
|   2  |Muss             |F     | Als ein Benutzer möchte ich, dass man von Pizzaschaufeln erschlagen werden kann, damit ich gestresst wird. |
|   3  |Kann             |R     | Als ein Benutzer möchte ich, dass man gute Musik hört wird, damit ich länger konzentriert bleibe. |
|   4  |Kann             |Q     | Als ein Benutzer möchte ich, dass man verschiedene Schwierigkeitsstufen auswählen kann, damit es auf mich anpassbar ist. |
|   5  |Muss             |F     | Als ein Benutzer möchte ich, dass man Essen zubereiten kann, damit das Spiel einen Sinn hat. | 
|   6  |Kann             |Q     | Als ein Benutzer möchte ich, dass man, wenn man zu viel Tomatensauce aufnimmt, die Sicht eingegrenzt wird, damit es schwerer wird. | 
|   7  |Kann             |R     | Als ein Benutzer möchte ich, dass man Item aufsammeln kann, damit meine Pizza individuell ist. | 
|   8  |Kann             |R     | Als ein Benutzer möchte ich, dass man im Shop sein Münzen loswerden kann, damit ich sie öfters sammle. | 
|   9  |Muss             |Q     | Als ein Benutzer möchte ich, dass man Superitems aufsammeln kann, damit der Spielspass erhöht wird. | 
|  10  |Muss             |F     | Als ein Benutzer möchte ich, dass man Hindernissen ausweichen muss, damit es eine Herausforderung ist. |
|   11 | Kann            | Q    | Als ein Benutzer möchte ich, dass man ein schön gestaltetes Startmenü hat, damit man schon einen Vorgeschmack bekommt |
|   12 |Kann             | R    | Als ein Benutzer möchte ich, dass es eine kleine Auswahl von Skins hat, damit man selber entscheiden kann wie man aussieht |
|   13 | Muss            | Q    | Als ein Benutzer möchte ich, dass die Map passend gestaltet ist, damit es das Perfekte Feeling gibt |
|   14 | Kann            | Q    | Als ein Benutzer möchte ich, dass es eine fixierte Sicht gibt, damit, man diese nicht aus Versehen verstellen kann |




### 1.3 Testfälle
| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |Spiel gestartet|Losrennen|Man kann endlos rennen|
| 2.1  |Spiel gestartet|Losrennen|Pizzaschaufel fliegt auf einen runter|
| 3.1  |Spiel starten|Im Startbildschirm warten|Es wird Musik gespielt|
| 4.1  |Spiel gestartet|Auswahl der Schwierigkeiten| Der richtige Modus wird gestartet|
| 5.1  |Spiel gestartet, Run begonnen|Man sammelt die Zutaten| Am Ende wird die Pizza gebacken|
| 6.1  |Spiel gestartet, genug Tomatensauce | Man nimmt Tomatensauce auf| Die Sicht wird verschlechtert|
| 7.1  |Spiel gestartet|Man rennt und sammelt die verschiedenen Items auf| Eine individuelle Pizza wird erstellt |
| 8.1  |Spiel gestartet, Münzen gesammelt|Man klickt im Startbildschirm auf "Shop"| Man wird zum Ingame Shop weitergeleitet|
| 9.1  |Spiel gestartet, Run gestartet|Super Item aufgesammelt|Man bekommt eine temporäre Superfähigkeit|
| 10.1 |Spiel gestartet. Run gestartet|Ausweichen eines Hindernis|Man überlebt und rennt weiter|
| 11.1 |  -  | Spiel starten  | Das Startmenü wird angezeigt |
| 12.1 | Spiel starten, Shop öffnen |Skin kaufen| der neue Skin wird ausgewählt |
| 13.1 | Spiel starten | Run starten | Ein passende Map wird gezeigt |
| 14.1 | Spiel starten, Run gestartet | Versuchen die Kameraperspektive zu verstellen | Erfolglos, die Kamera bleibt da |



### 1.4 Diagramme
![image](https://user-images.githubusercontent.com/111044137/220881321-3fe59366-10a5-4ab2-9267-11162573eead.png)
![image](https://user-images.githubusercontent.com/111044137/222373448-4eded339-9682-43e2-b4cc-e55ee57d08b3.png)



## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
|1a|09.03.2023|Müller,Broder|Grundgerüst der Map erstellen|4 AP|
|1b|09.03.2023|Aeschlimann,Spaqi|Eine Figur Programmieren|4 AP|
|1c|09.03.2023|Aeschlimann,Spaqi|Die animierte Figur zum Laufen programmieren |3 AP|
|2a|09.03.2023|Müller,Broder| Pizza schaufeln programmieren, die vom Himmel fallen|3 AP|
|2b|09.03.2023|Müller,Broder|Pizzaschaufel schaden berechnen.|2 AP|
|3a|06.04.2023|Müller,Broder|Musik heraussuchen und ins Spiel einfügen|2 AP|
|4a|16.03.2023|Aeschlimann,Spaqi|Schwierigkeitsstufen erstellen|4 AP|
|5a|16.03.2023|Aeschlimann,Spaqi|Einzelne Zutaten programmieren, die man beim darüber gehen einsammeln kann|4 AP|
|5b|16.03.2023|Müller,Broder|verschiedene Pizzen programmieren, die man zubereiten kann|4 AP|
|6a|23.03.2023|Müller|Tomatensauce erstellen und zufällig auf der Map verteilen|4 AP|
|6b|23.03.2023|Broder|Programmieren das ab einer gewissen Anzahl Tomatensauce die Sicht eingeschränkt wird.|4 AP|
|7a|23.03.2023|Aeschlimann,Spaqi|mehrere Items erstellen, die man beim darüber gehen einsammeln kann|4 AP|
|7b|23.03.2023|Müller,Broder|mehrere verschiedene Pizzen erstellen, die man mit verschiedenen Zutaten zubereiten kann|4 AP|
|8a|23.03.2023|Aeschlimann|Münzen Programmmieren, die man beim darüber gehen einsammelt|3 AP|
|8b|30.03.2023|Aeschlimann,Spaqi|Einen Shop erstellen, in dem man die Münzen ausgeben kann|3 AP|
|9a|30.03.2023|Müller,Broder|Superitems programmieren und zufällig verteilen|2 AP|
|9b|30.03.2023|Müller,Broder|Die einzelnen Superfähigkeiten programmieren|4 AP|
|10a|30.03.2023|Aeschlimann,Spaqi|Hindernisse erstellen und auf der Map verteilen|4 AP|
|10b|30.03.2023|Aeschliman,Spaqi|Programmieren das die Figur sich bewegen kann|4 AP|
Total: 64 AP



## 3 Entscheiden
09.03.2023, 10:00, Wir hatten verschiedenste Fehler und Bugs in Unity. Unser Projekt stellt sich als schwieriger heraus, als wir es uns vorgestellt haben. 
16.03.2023, 9:20, Unser ganzer Prototyp ist abgestürzt. Wir müssen jetzt schauen ob wir diesen wieder neu programmieren können, allerdings wird uns das viel Zeit kosten.
23.03.2023, 9:30, Unser Prototyp steht zwar wieder, ist aber immernoch lange nicht fertig (keine Map, Hindernisse)
## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
|1.A|09.03.2023|Müller,Broder|90min|240min|
|1.B|09.03.2023|Aeschlimann,Spaqi|90min|120min|
|1.C|09.03.2023|Aeschlimann,Spaqi|45min|120min|
|2.A|16.03.2023|Müller,Broder|45min|-|
|2.B|16.03.2023|Müller,Broder|45min|-|
|3.A|16.03.2023|Müller,Broder|45min|-|
|4.A|16.03.2023|Aeschlimann,Spaqi|90min|-|
|5.A|23.03.2023|Aeschlimann,Spaqi|90min|-|
|6.A|23.03.2023|Müller|45min|-|
|6.B|23.03.2023|Broder|45min|-|
|7.A|23.03.2023|Aeschlimann,Spaqi|90min|-|
|7.B|23.03.2023|Aeschlimann,Spaqi|90min|-|
|8.A|23.03.2023|Aeschlimann,Spaqi|45min|-|
|8.B|30.03.2023|Aeschlimann,Spaqi|45min|-|
|9.A|30.03.2023|Müller,Broder|45min|-|
|9.B|30.03.2023|Müller,Broder|90min|-|
|10.A|30.03.2023|Aeschlimann,Spaqi|45min|-|
|10.B|30.03.2023|Aeschlimann,Spaqi|45min|-|


## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester | Fazit |
| ---- | ----- | -------- | ------ |-|
| 1.1  | 03.04.23      | Funktioniert         | Spaqi       |- |
| 2.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 3.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 4.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 5.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 6.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 7.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 8.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 9.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 10.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 11.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 12.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 13.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |
| 14.1  | 03.04.23      | Funktioniert nicht         | Spaqi       |- |


Wir haben uns am 9.3 entschieden das unser Projekt 3D sein sollte.
✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
