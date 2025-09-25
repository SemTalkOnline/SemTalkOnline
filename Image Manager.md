# SemTalk Online and images

SemTalk Online allows users to visually enhance models by integrating associated images into model diagrams.

Most modeling templates include stencils that contain images that are shown on modeling worksheets. Images can be associated with specific modeling methodology components or they can be user-defined pictures.

![Bildsymbol in der Schablone](./images/bildermanager/bildschablone.PNG)

Image files can be integrated in different ways:

* Via external hyperlinks: This is used for images that are stored and uploaded from a central file location. Changes, deletions and access restrictions made to the primary image are propagated to all instances of the image in all models that contain the image. A core benefit of this approach is that external hyperlinks do not affect the size of the model file.

* Via embedded base64-encoded image strings: Images can be permanently integrated into the model file as base64-encoded character strings. Please refer to section: [Convert images to base64](./image-manager#convert-images-to-base64)!
The primary advantage of this method is that the image does not have to be loaded from an external source so it is always immediately accessible to every model user. A disadvantage is that if any changes are made to the image, changes will not be propagated to the other models and model diagrams where the object is used. Additionally, model files can quickly become very large (even too large) if the model contains embedded images. Embedded objects should be used for images that do not change often, images that are specific to individual models and/or those images that cannot be obtained from a reliable external source.

* As a unique symbol: Images can be added directly to model diagrams. This makes sense if an image only appears once in the model. 

* Via an integraded image administration interface - the Image Manager: If you are working with many images and, if these images are reused in several places, Image Manager is the best interface for images. All images can be clearly created here and transferred to the file. In this way, several modelers can contribute images and manage them together so that they are available for all modeling needs. 

# Integrating Images as Symbols

Diese Variante gilt ausschließlich für Bilder, die als Hyperlink eingefügt werden sollen.
Ist ein Bild Symbol auf dem Zeichenblatt platziert, kann durch Doppelklick auf den Namen "Bild", den das Symbol initial bekommen hat, einfach ein Hyperlink als Text eingefügt werden.
Mit Enter oder klick an eine andere Stelle wird die Url übernommen und das Bild wird angezeigt.

![Bild als Hyperlink am Symbol einfügen](./images/bildermanager/bildurlamsymbol.png)


# Bilder über den Formatierungsdialog hinzufügen

Ist ein Bild Symbol auf dem Zeichenblatt platziert, kann mit Rechtsklick --> Formatierung (oder Menü Symbol-->Formatierung) der Formatierungsdialog geöffnet werden. Dieser besitzt den Tab "Bild".

![Formatierung Tab Bild öffnen](./images/bildermanager/bildformatierung.PNG)

Hier kann entweder ein externer Hyperlink angegeben werden oder eine nach base64 konvertierte Bilddatei eingebettett werden. Dazu lesen Sie bitte wieder den Abschnitt: [Bilder nach base64 konvertieren](./Bilder-Manager#bilder-nach-base64-konvertieren)!

Danach kann das Bild in die Datei eingebettet werden.

Wird im Feld ID ein Name für das Bild eingetragen ist das angelegte Bild danach auch im Formatierungsdialog anderer Bild Symbole über die Auswahlbox mit dem Label ID wiederverwendbar.


# Der Bildermanager

## Den Bildermanager öffnen

Über den Menüpunkt Extras --> Anpassen --> Bildermanager wird der Bildermanager geöffnet.
![BilderManager öffnen](./images/bildermanager/bildermanager.png)

![BilderManager Oberfläche](./images/bildermanager/bildermanagercontrol.PNG)

Im nun geöffneten Fenster werden dann alle existierenden Bilder der Datei mit Namen, Inhalt, Größe und ob es bereits in der Datei gespeichert ist aufgelistet. 
Für das Arbeiten mit Bildern bietet die Menüleiste verschiedenste Optionen.

## Die Bildermanager Menüleiste

![BilderManager Oberfläche](./images/bildermanager/bildermanagermenue.png)

* Neu (+ Symbol): Erlaubt das Anlegen eines neuen Bilder im Bildermanager
* Bearbeiten (Stift Symbol): Vorhandene Bilder können bearbeitet werden
* Löschen (Papiereimer Symbol): Bilder können gelöscht werden
* Für Datei übernehmen: Sollen Bilder auch wirklich in die Datei eingebettet werden, müssen diese einmal für die Datei übernommen werden und stehen danach für due Nutzung bereit
* Aus der Datei entfernen: Bilder können aus der Datei wieder entfernt werden. Werden diese bereits verwendet, so verliert das entsprechende Bilder-Shape seinen Inhalt. Ob ein Bild in der Datei gespeichert ist, lässt sich anhand der Spalte "Datei" im Übersichtsmenü des Bildermanagers erkennen.
* Export/Import: Die Konfiguration aus dem Bildermanager kann exportiert bzw. importiert werden, um einen Satz Bilder einfach auf andere Modelledateien übertragen werden kann

## Arbeiten mit dem Bildermanager

Der Bildermanager listet alle vorhandenen Bilder auf. Es gilt jedoch zu beachten dass Bilder, die über den Bildermanager angelegt wurden, initial nur im Bildermanager des aktuell geöffneten Modelles existieren. Um ein oder mehrere Bilder in die Datei zu übernehmen, muss der Menüeintrag "Für Datei übernehmen" betätigt werden. Erst danach sind die Bilder im Modell eingebettet. Dieses Vorgehen stellt sicher dass die Bilder zuerst korrekt angelegt und kontrolliert werden können bevor sie Auswirkungen auf die Modelldatei haben. Genauso lassen sich die Bilder dann auch wieder zentral aus der Datei entfernen indem "Aus der Datei entfernen" im Menü geklickt wird.

Bilder, die in die Datei eingebettet sind, besitzten in der Spalte Datei ein Häkchen.

Um ein neues Bild hinzuzufügen bzw. ein vorhandenes zu bearbeiten nutzen Sie die "Neu" oder "Bearbeiten" Buttons aus der Menüleiste. Ein Bildereintrag besteht immer aus einer ID, also einem eindeutigen Namen, und dem Bilderinhalt im Feld "Bild". Dabei kann es sich entweder um eine Url oder die base64 konvertierte Zeichenkette eines Bilder handeln.

Werden viele als base64 eingebettete Bilder verwendet gilt es auch ein Auge auf die Größe der Bilder zu haben. Je mehr Bilder in der Modelldatei gespeichert werden, desto größer wird diese auch und kann zu längeren Ladezeiten führen. Auch beim Export des Modelles in eine Veröffentlichungsdatenbank kann es zu Problemen kommen, wenn die Datei zu groß wird. Daher ist die Dateigröße für den Export auf ca. 10 Mb beschränkt. SemTalk Online wird ab einer Größe von ca. 7 Mb diesbezüglich eine Warnmeldung im Bildermanager anzeigen. Soll kein Export in eine Veröffentlichungsdatenbank durchgeführt werden, kann die Warnung ignoriert werden.



# Bilder nach base64 konvertieren

Um ein Bild in einem SemTalk Online Modell einzubetten muss die Datei in eine base64 Zeichenkette umkonvertiert werden.
SemTalk Online bietet dafür kein eigenes Konvertierungswerkzeug an, sondern verlinkt auf ein freizugängliches unter https://base64.guru/converter/encode/I. Konverter anderer Anbieter können aber ebenso genutzt werden.

![base64 konvertieren](./images/bildermanager/konverter.PNG)

Für die Konvertierung muss das Bild einmal in den Konvertierungsservice hochgeladen werden, das Output Format auf "Data URI -- data:content/type;base64" gestellt werden und dann der Encode Knopf gedrückt werden. 
Das Ergebnis kann dann nach SemTalk Online in das Feld "Bild" kopiert werden. Hat der Vorgang geklappt zeigt SemTalk Online auch direkt eine Vorschau des Bildes im Dialog an.





