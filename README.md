# Gruppenarbeit INF22A BWL

Für die gemeinsame Zusammenstellung aller Themen ist es einfacher jeder pushed sein Abstract. Ihr müsst dazu mindestens 2 Dateien ändern, falls ihr auf Literatur verweisen wollt, sind es 3.

## Wichtige Dateien

| Datei         | Bedeutung                                                                                    |
|---------------|----------------------------------------------------------------------------------------------|
| main.tex      | Hauptdatei mit include Befehlen zu euren einzelnen Abstracts.                                |
| literatur.bib | Literaturverzeichnis, hier kommen eure Quellen rein.                                         |
| abstracts/    | Hier liegen eure Abstracts in .tex Form. Dieses müsst ihr anlegen und in main.tex verlinken. |


Ich habe meine Zusammenfassung schon eingefügt (nur als Muster, ich habs noch nicht angefangen, aber auch mit Literaturverweiß, dass man sieht, wie es geht), da könnt ihr euch ein Beispiel nehmen.

## How to

Kleine Schritt für Schritt Anleitung wie ihr das machen könnt. Geht bestimmt mit Windows auch auf der Command Line ansonsten einfach in der virtuelle Maschine machen.

1. SSH Key anlegen (https://gist.github.com/xirixiz/b6b0c6f4917ce17a90e00f9b60566278)

1. Irgendein Ordner lokal anlegen. Dort reinwechseln.

1. Lokal Repo laden mit Befehl:
    git clone https://github.com/ben165/Gruppenarbeit_INF22A.git

1. Neuer Branch erstellen und dahin wechseln (MeinAbstract als Beispiel):
    git checkout -b MeinAbstract

1. Änderung in Dateien vornehmen (main.tex - hier input hinzufuegen, literatur.bib) und eigenes Abstract als *Dateinamen.tex* in Ordner *abstracts/* hinzufügen. Ich habe für den Dateinamen meine Initialien verwendet und daraus die Datei *bu.tex* erstellt. Diese muss einzigartig sein.

1. Eure geaenderten Dateien hinzufuegen (sofern eine Aenderung gemacht wurde):
    git add abstracts/MEINABSTRACT.tex
    git add main.tex
    git add literatur.bib

1. Nach getaner Arbeit Wechsel in den main branch
    git checkout main

1. Main branch updaten falls jemand was gaendert hat:
    git pull

1. Zurueck in den eigenen Branch
    git checkout MeinAbstract

1. Main auf MeinAbstract mergen
    git merge origin/main

1. Dann pushen
    git push origin MeinAbstract

