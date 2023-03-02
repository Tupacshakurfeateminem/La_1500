# Projekt-Dokumentation

☝️ Alle Text-Stellen, welche mit einem ✍️ beginnen, können Sie löschen, sobald Sie die entsprechende Stellen ausgefüllt haben.

Daisy: Ben Müller,John Broder, Brandon Spaqi, Christian Aeschlimann

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 23.02.2023| 0.0.1   | Heute haben wir uns unser Thema Pizza runner erfunden und einige Ideen darüber gesammelt, auserdem haben wir mit den User-Stories angefangen und das Pap gemacht.
|       | ...     |                                                              |
|       | 1.0.0   |                                                              |

## 1 Informieren

### 1.1 Ihr Projekt

In diesem Programmierprojekt programmieren wir einen Endless-Runner, bei dem man eine Pizza belegt, in dem man die richtigen Zutaten einsammelt. 

Wir wollen mithilfe von Unity einen Endless-Runner programmieren, bei dem man verschiedenen Hindernissen ausweichen muss und gleichzeitig eine Pizza macht, in dem man verschiedene Zutaten einsammeln muss. Wenn eine Pizza fertig belegt ist, bekommt man einen Pizzapunkt und fängt wieder mit einer neuen Pizza an. Während man rennt, fallen in regelmässigen Abständen Pizzaschaufeln vom Himmel, denen man dann ausweichen muss. Neben der exponentiell steigenden Geschwindigkeit des Users, erhöht sich auch die Geschwindigkeit, in dem die Schaufeln vom Himmel fallen. Falls der User eine Zutat zum zweiten Mal einsammelt, wird er «bestraft». Wir haben uns final für 3 Schwierigkeitsmodi entschieden. 


### 1.2 User Stories
| US-№ | Verbindlichkeit | Typ  | Beschreibung                      |
| ---- | --------------- | ---- | ---------------------------------- |
|   1  |Muss             |F     | Als ein Benutzer möchte ich dass, man endlos rennen kann, damit ich Spass habe. | 
|   2  |Muss             |F     | Als ein Benutzer möchte ich dass, man von Pizzaschaufeln erschlagen werden kann, damit ich gestresst wird. |
|   3  |Kann             |R     | Als ein Benutzer möchte ich dass, man gute Musik hört wird, damit ich länger konzentriert bleibe. |
|   4  |Kann             |Q     | Als ein Benutzer möchte ich dass, man verschiedene Schwierigkeitsstufen auswählen kann, damit es auf mich anpassbar ist. |
|   5  |Muss             |F     | Als ein Benutzer möchte ich dass, man Essen zubereiten kann, damit das Spiel einen Sinn hat. | 
|   6  |Kann             |Q     | Als ein Benutzer möchte ich dass, man wenn man zu viel Tomatensauce aufnimmt die Sicht eingegrenzt wird, damit es schwerer wird. | 
|   7  |Kann             |R     | Als ein Benutzer möchte ich dass, man Item aufsammeln kann, damit meine Pizza individuell ist. | 
|   8  |Kann             |R     | Als ein Benutzer möchte ich dass, man im Shop sein Münzen loswerden kann, damit ich sie öfters sammle. | 
|   9  |Muss             |Q     | Als ein Benutzer möchte ich dass, man Superitems aufsammeln kann, damit der Spielspass erhöht wird. | 
|  10  |Muss             |F     | Als ein Benutzer möchte ich dass, man Hindernissen ausweichen muss, damit es eine Herausforderung ist. |
✍️ Jede User Story hat eine ganzzahlige Nummer (1, 2, 3 etc.), eine Verbindlichkeit (Muss oder Kann?), und einen Typ (Funktional, Qualität, Rand). Die User Story selber hat folgende Form: *Als ein 🤷‍♂️ möchte ich 🤷‍♂️, damit 🤷‍♂️*.

### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |              |         |                   |
| ...  |              |         |                   |

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, die der Testfall abdeckt, und `m` von `1` an nach oben gezählt. Beispiel: Der dritte Testfall, der die zweite User Story abdeckt, hat also die Nummer `2.3`.

### 1.4 Diagramme
![image](https://user-images.githubusercontent.com/111044137/220881321-3fe59366-10a5-4ab2-9267-11162573eead.png)
![image](https://user-images.githubusercontent.com/111044137/222373448-4eded339-9682-43e2-b4cc-e55ee57d08b3.png)

✍️Fügen Sie hier ein Use Case-Diagramm mit mindestens 10 Anwendungsfällen ein; und einen PAP.

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
|1a| 09.03.2023|6| Grundgerüst der Map erstellen|90min|
|1b|09.03.2023|8|  Eien Figur Programmieren|90|
|1c|09.03.2023|l|Die animierte Figur zum laufen programmieren |60|
|2a| 9.02.2023|2| Pizza schaufeln programmieren die vom Himmel fallen|90|
|2b|09.02.2023|2|Pizza schaufel schaden berechnen.|90|
|3a|09.03.2023|2|Musik raussuchen und ins Spiel einfügen|90|
|4a|09.03.2023|2|schwierigkeitsstuffen erstellen|90|
|5a|09.03.2023|2|Einzelne Zutaten programmieren die man beimdarüber gehen einsammeln kann|90
|5b|09.03.2023|2|verschiedene Pizzen programmieren die man zubereiten kann|90|
|6a|09.03.2023|2|Tomaten sauce erstellen und zufällig auf der Map verteilen|90|
|6b|09.03.2023|2|Programmieren das ab einer gewissen anzahl Tomaten sauce die sicht eingeschränkt wird.|90|
|7a|09.03.2023|2|mehrere Items erstellen die man beim darüber gehen einsammeln kann|90|
|7b|09.03.2023|2|mehrere verschiedene Pizzen erstellen die man mit verschiedenen Zutaten zubereiten kann|90|
|8a|09.03.2023|2|Münzen programmmieren die man beim darüber gehen einsammelt|90|
|8b|09.03.2023|2|Einen Shop erstellen in dem man die Münzen ausgeben kann|90|
|9a|09.03.2023|2|Superitems programmieren und zufällig verteilen|90|
|9b|09.03.2023|2|Die einzelnen superfähigkeiten programmieren|90|
|10a|09.03.2023|2|Hindernisse erstellen und auf der Map verteilen|90|
|10b|09.03.2023|2|Programmieren das die Figur sich bewegen kann|90|
Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
