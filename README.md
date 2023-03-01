# Gruppenarbeit INF22A BWL

Für die gemeinsame Zusammenstellung aller Themen ist es einfacher jeder pushed sein Abstract. Ihr müsst dazu mindestens 2 Dateien ändern, falls ihr auf Literatur verweisen wollt, sind es 3.

## Wichtige Dateien

| Datei         | Bedeutung                                                                                    |
|---------------|----------------------------------------------------------------------------------------------|
| main.tex      | Hauptdatei mit include Befehlen zu euren einzelnen Abstracts.                                |
| literatur.bib | Literaturverzeichnis, hier kommen eure Quellen rein.                                         |
| abstracts/    | Hier liegen eure Abstracts in .tex Form. Dieses müsst ihr anlegen und in main.tex verlinken. |


Ich habe meine Zusammenfassung schon eingefügt (nur als Muster, ich habs noch nicht angefangen, aber auch mit Literaturverweiß, dass man sieht, wie es geht).

## How to

Kleine Schritt für Schritt Anleitung wie ihr das machen könnt. Geht bestimmt mit Windows auch auf der command line ansonsten einfach in der virtuelle Maschine machen. Ihr braucht einen GutHub Account und einen SSH Key, den ihr im Profil auf GitHub hinterlegen müsst.

1. Bei GitHub anmelden, SSH Key anlegen (https://gist.github.com/xirixiz/b6b0c6f4917ce17a90e00f9b60566278) und im Profil einpflegen.

1. Irgendein Ordner lokal anlegen. Dort reinwechseln.

1. Lokal Repo laden mit Befehl:

    `git clone https://github.com/ben165/Gruppenarbeit_INF22A.git`

1. Neuer Branch erstellen und dahin wechseln (MeinAbstract als Beispiel):

    `git checkout -b MeinAbstract`

1. Änderung in Dateien vornehmen (**main.tex** - hier dein input hinzufuegen, **literatur.bib**) und eigenes Abstract als **Dateinamen.tex** in Ordner **abstracts/** hinzufügen. Ich habe für den Dateinamen meine Initialien verwendet und daraus die Datei **bu.tex** erstellt. Diese muss einzigartig sein.

1. Eure geaenderten Dateien hinzufuegen (sofern eine Aenderung gemacht wurde):

    `git add abstracts/MEINABSTRACT.tex`

    `git add main.tex`

    `git add literatur.bib`

1. Nach getaner Arbeit einen Commit absetzen mit Inhalt was geaendert wurde:

    `git commit -m "Update Abstract Benjamin"`

1. Zurück in den main branch

    `git checkout main`

1. Main branch updaten falls jemand was gaendert hat:

    `git pull`

1. Zurück in den eigenen Branch

    `git checkout MeinAbstract`

1. Main auf MeinAbstract mergen

    `git merge origin/main`

1. Dann pushen

    `git push origin MeinAbstract`


Ich glaube, man muss nicht unbedingt aus dem momentanen Branch auschecken, um main zu aktualisieren. Bin mir mit der Befehlsreihenfolge nicht so sicher. Wenn ihr euren Branch pusht, pflege ich das auf GitHub dann final ein. Versucht nicht so viel in den Dateien **main.tex** und **literatur.bib** zu editieren, da hier die meisten Konflikte entstehen können.

Als Beispiel die **main.pdf** als momentan kompilierte Datei. Ihr könnt ja zum Test mal eure Überschrift in eurer **abstract** Datei einfügen und pushen, damit ihr versteht, wie das geht.

Mir fällt sonst kein besserer Weg ein wie man das machen kann.

Cheers
