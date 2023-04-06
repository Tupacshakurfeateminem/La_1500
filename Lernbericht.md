# Lern-Bericht
Daisy: Ben Müller, John Broder, Brandon Spaqi, Christian Aeschlimann

## Einleitung
In unserem Projekt haben wir versucht, einen Endless-Runner zu programmieren. Dabei haben wir uns Spielen wie *SubwaySurfers* oder *TempleRun* inspirieren lassen. 


## Was habe ich gelernt?

In diesem Projekt haben wir uns explizit damit beschäftigt, wie man eine Endless-Map  programmiert und gegebenenfalls designt.

## Beschreibung


Das Prinzip einer Endless-Map ist eigentlich ganz einfach. Man hat ein grosses Map-Tile, das schön designt ist und abwechslungsreich gestaltet ist (*Bild, Nr. 1*). Dann programmiert man diese Tile so, dass es, sobald der Spieler im letzten Ende des ersten Mapabschnittes ist, ein neuer Abschnitt erscheint (*Bild, Nr. 2*), auf den der Spieler übergangslos rüberlaufen kann. Sobald der Spieler auf das neue Tile gelaufen ist, wird das alte Tile gelöscht (*Bild, Nr. 3*). So spart man enorm viel Performance des Computers und Zeit, die man sonst mit dem Designen der Map verbringen würde.  
![image](https://user-images.githubusercontent.com/111043950/230325346-e64b710b-94aa-4e12-b8a4-a109682b5263.png)

Hier ist ein Codebeispiel für eine Endless-Map. Mithilfe der Updatefunktion checkt der Code, ob der Spieler schon bei dem vorgegebenen Punkt ist, und falls das der Fall sein sollte, setzt er ein neues Tile an das Ende des alten. Anschliessend wird das alte Tile gelöscht, um Performance einzusparen.
   

    void Start()
    {
        activeTiles = new List<GameObject>();
        for (int i = 0; i < tilesOnScreen; i++)
        {
            SpawnTile();
        }
    }

    void Update()
    {
        if (player.position.z > (activeTiles[lastIndex].transform.position.z - tileLength / 3))
            SpawnTile();
    }

    void SpawnTile()
    {
        GameObject tile = Instantiate(mapTiles[Random.Range(0, mapTiles.Length)]);
        tile.transform.position = Vector3.forward * (++lastIndex * tileLength);
        activeTiles.Add(tile);
        if (activeTiles.Count > tilesOnScreen)
        {
            Destroy(activeTiles[0]);
            activeTiles.RemoveAt(0);
        }
    }


 
So könnte eine einfache Version einer Endless-Map in einem Endless-Runner aussehen: 
![Pizza_runner_gif](https://user-images.githubusercontent.com/111043950/230328082-5842d2f3-5ea4-4ad3-ac94-32a233cfae6b.gif)

 
## Verifikation

In dem GIF kann man sehen, dass wir eine Endless-Map programmiert haben, auf dieser sind auch Coins verteilt. In dem Bild kann man auch erkennen wie wir vorgegangen sind, zuerst hatten wir andere Ideen. Dann wäre die Map allerdings nicht endless geworden, darum haben wir einen Map-Tile geschrieben, das dann dupliziert und das alte Tile löscht.  In dem Code sieht man, wie wir dies programmiert haben. Kurz zusammengefasst muss die Person einen gewissen Punkt erreichen, damit ein neues Map Teil erstellt oder gelöscht wird.

# Reflexion zum Arbeitsprozess

+In diesem Projekt waren wir recht gut organisiert und wollten viel lernen.  Wir waren sehr kreativ und haben uns mehrere verschiedene Projekte vorgestellt, am Ende war   es dann aber der Pizza Runner der sich durchsetzen konnte.

-Unsere Effizienz beim Coden könnte man noch verbessern, allgemein war für uns alle Unity etwas Neues. Aus diesen Gründen konnten wir unser Projekt nicht wie gewünscht    beenden.

**VBV**:  Wir werden uns nächstes Mal besser vorbereiten müssen, damit wir in der Zeit, die wir haben wissen, was und wie wir etwas programmieren müssen.
