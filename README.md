# 3D-Drucker-11-462

## Einrichtung

### Installieren von OrcaSlicer
Um mit dem 3D-Druck zu beginnen, benötigen Sie OrcaSlicer. Diese Software hilft Ihnen dabei, Ihre 3D-Modelle für den Druck vorzubereiten. Sie können OrcaSlicer hier herunterladen:  
https://orca-slicer.com/

### Druckerprofil / Filamentprofile
Drucker- und Filamentprofile sind entscheidend, um eine optimale Druckqualität zu erreichen. Sie können diese Profile in OrcaSlicer unter „Datei“ → „Importieren“ → „Konfiguration importieren“ hinzufügen. Hier können Sie sowohl Drucker- als auch Filamentprofile importieren, die speziell auf Ihren Drucker und das verwendete Filament abgestimmt sind. Das Druckerprofiel sowie die dazugehörigen Filament profiele finden sie ine einer einzigen Orcadatei am anfange der Repositorys.  


## Vorbereitung

### Slicen
Um ein 3D-Objekt für den Druck vorzubereiten, müssen Sie es zuerst „slicen“. Öffnen Sie OrcaSlicer und laden Sie das gewünschte 3D-Modell (STL-Datei) in das Programm. Wählen Sie das passende Druckerprofil und das Filamentprofil aus. Stellen Sie alle Druckparameter entsprechend der Anwendung der Bauteils ein. Nachdem alle Parameter konfiguriert sind, klicken Sie auf „Slice“ und speichern Sie die G-Code-Datei.

#### 📝 Schichthöhe (Layer Height)
Die Schichthöhe bestimmt, wie dick jede gedruckte Lage ist. Kleinere Werte (z.B. 0,1 mm) liefern feinere Details, während größere Werte (z.B. 0,3 mm) den Druck beschleunigen. Als Standard für gute Qualität und moderate Druckzeit gilt 0,2 mm.

#### 📝 Wandlinienanzahl (Wall Line Count)
Dieser Wert gibt an, wie viele Linien die Außenwand eines Modells bilden. Mehr Wandlinien erhöhen die Stabilität und verbessern die Oberflächenqualität. Für die meisten Drucke sind 2–3 Linien ein guter Ausgangspunkt.

#### 📝 Fülldichte (Infill Density)
Die Fülldichte legt fest, wie stark das Innere des Modells gefüllt wird, angegeben in Prozent. Höhere Werte machen das Objekt stabiler und schwerer, niedrige Werte sparen Material und Zeit. Typische Bereiche liegen zwischen 10 % (Deko) und 30 % (mechanisch belastete Teile).

#### 📝 Anzahl oberer und unterer Schichten (Top/Bottom Layers)
Dieser Parameter steuert, wie viele volle Schichten oben und unten im Modell gedruckt werden. Zu wenige Schichten können zu Löchern oder unsauberen Oberflächen führen, besonders bei geringem Infill. Für saubere Ergebnisse sind 3–6 Schichten (bei 0,2 mm Layer Height) empfehlenswert.

### Drucker checken
Bevor Sie mit dem Druck beginnen, sollten Sie einige Punkte überprüfen, um sicherzustellen, dass der Druck reibungslos verläuft:

- **Ist das richtige Filament eingelegt?** ( wenn dies nicht der Fall ist kann die Exdruder temperatur manuel am Display eingestellt werden. Wenn die Temperatur ereicht ist kann das Alte Filamen entnommen und das neue Filament eingesetzt werden )
- **Ist die Druckplatte sauber?**
- **Ist der Druckraum frei von Hindernissen?**
- **Ist der Drucker eingeschaltet und bereit für den Start?**
- **Sind die Filamentrollen ordentlich eingelegt und ist noch genug Filament enthalten ?**
- **Sind die Druckparameter korrekt eingestellt?**

Diese Checkliste sorgt dafür, dass Sie nichts übersehen, bevor Sie mit dem Drucken beginnen.

## Drucken

### Zu Beachten 
- Die Drucke sollenten sich länger als 4 Studen dauer um zu gewährzuleisten das der Drucker jeden tag neu benutzt werden Kann. Sollten sie längere drucke haben bitte wenden sie sich an Feldmann@rptu.de
- Sollten andere Probleme auftretten bitte sie sich auch hier an Feldmann@rptu.de
  

### Drucker bedienen und Datei hochladen
Nach dem Slicen können Sie mit dem Drucken beginnen. Die Bedienoberfläche von **Mainsail** und **Klipper** ist intuitiv gestaltet und ermöglicht eine einfache Steuerung des Druckers. Auf dem **Mainsail Dashboard** finden Sie Optionen wie „Druck starten“, „Temperatur einstellen“ und „G-Code hochladen“. 

Um die Datei direkt nach dem Slicen in OrcaSlicer auf den Drucker zu laden, klicken Sie einfach auf „Aktuelle Platte Drucken“ und wählen Sie zwischen "Hochlade" und "Drucken und hochladen" aus, bei zweiteren wird der druck direkt gestartet. Alternativ können Sie die G-Code-Datei auch auf das Mainsail-Interface hochladen und den Druck direkt über das Web-Interface starten. Fall der Drucker nicht ereichbar ist hat sich die IP adresse verändert, diese Können sie am Touchdisplay des Druckers unter Netzwerke einsehen. Zum aktualiesieren der IP drücken sie auf das Wlan Symbol neben dem ausgewählten drucker und geben die neue IP ein. 

Sollten sie einen Druck wiederholen wollen müssen sie diesen nicht neu Slicen. Sie könne einfach am Touchdisplay unter Print den Druck erneut Starten.






