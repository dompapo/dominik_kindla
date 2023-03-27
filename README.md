Klient Gerald:

Ermöglichen Sie ihrem Klienten die Steuerung des PCs mittels Kamera. Er soll über diese das AsTeRICS Grid ansteuern können sowie einen Browser bedienen können und ggf. E-mails schreiben. (Tastatureingaben!)

Für das ACS und ARE wurde eine Modell gebraucht für die Übertragung von Daten vom Asterics Grid and das Openhab und somit an die Jalousien und Lichet in der Küche. Im Folgenden Bild wird das Mordell dargestellt. Das Modell wurde in der Asterics Configuration Suite erstellt.
![Asterics Configuration Suite](https://user-images.githubusercontent.com/129118598/228075509-f4c8ee07-9f62-4035-b24f-abbe2764d30c.PNG)

Um Daten vom AsTeRICS Grid an OpenHAB zu übertragen und somit Jalousien und Lichter in der Küche zu steuern, wurde ein Modell in der AsTeRICS Configuration Suite erstellt. Das Modell wird im folgenden Bild dargestellt und ist erforderlich für die Integration von ACS und ARE.

Um die Verbindung zwischen dem AsTeRICS Grid und OpenHAB herzustellen, musste der OpenHAB-Block angepasst werden, indem der Hostname und der Port geändert wurden. Die entsprechenden Änderungen wurden in den OpenHAB-Einstellungen vorgenommen.
![Openhab](https://user-images.githubusercontent.com/129118598/228075786-317f7987-6518-4baf-a82d-5c356bdb65aa.PNG)

Da der Klient die Maus mithilfe einer Kamera steuern kann, wurde das Startup-Programm der AsTeRICS Runtime Environment (ARE) verwendet. Das Programm sieht wie folgt aus:
![AsTeRICS](https://user-images.githubusercontent.com/129118598/228075546-d878fc68-25b7-4a58-9c27-2cfbf33012b2.PNG)


Für die Steuerung wurde ein AsTeRICS Grid erstellt, das wie folgt aussieht:
![Grid](https://user-images.githubusercontent.com/129118598/228075558-c2d52968-4453-4840-b15d-fbe8c6247a27.PNG)


Um das AsTeRICS Grid mit OpenHAB zu verbinden, musste zunächst das ACS-Modell heruntergeladen werden. Dadurch war es möglich, den Block im Modell auszuwählen. Die Daten für die Jalousien wurden aus einem PDF-Dokument entnommen. Jeder Datentyp besteht aus "@OPENHAB: GERÄT, Variable". Im Fall der Jalousien gab es die Variablen "UP", "DOWN" und "40".
![Jalousien](https://user-images.githubusercontent.com/129118598/228076180-9565ae7d-e143-461a-a40d-53fc203f6419.PNG)

Für die Lichter in der Küche wurde dasselbe Verfahren wie für die Jalousien angewendet. Nach dem Herunterladen des ACS-Modells konnte der Block ausgewählt und die Daten eingetragen werden. Die Optionen für die Variablen sind entweder "OFF" oder "ON".
![Lichter](https://user-images.githubusercontent.com/129118598/228076171-7d8ea9d9-a102-41e5-a95b-72f92fdd6763.PNG)

Der Kunde wünschte sich außerdem die Möglichkeit, ein Radio über das AsTeRICS Grid zu bedienen. Zu diesem Zweck wurde ein anderes Grid erstellt. Das Radio-Grid ermöglicht ihm, Sender auszuwählen, die Lautstärke zu erhöhen oder zu verringern und das Radio auszuschalten. Im folgenden Bild sind die Einstellungen für die Senderauswahl dargestellt:
![Radio](https://user-images.githubusercontent.com/129118598/228076155-99cd1d77-68f6-42fb-82f5-dd1782569a57.PNG)

![RadioEinstellungen](https://user-images.githubusercontent.com/129118598/228076111-2db1fafa-e32c-490b-9f10-29438f3e78e1.PNG)



Videos zur Bedienung des Grids und zur Verwendung der Bildschirmtastatur zum Schreiben von E-Mails sind in den hochgeladenen Dateien enthalten.
