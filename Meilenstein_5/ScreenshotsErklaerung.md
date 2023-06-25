# Login

Zum Einloggen in ein Account muss man Benutzername und Passwort eingeben. Mittels Abfrage an die Datenbank (SQLite) soll überprüft werden, ob ein Nutzer mit den eingegeben Nutzernamen und Passwort existiert. Einen Account kann man auf der Registrieren-Activity anlegen indem man auf dem Registrieren-Button drückt.

<img src="./Screenshots/Anmelden.png" alt="Bildbeschreibung" style="width: 200px; height: auto;">


# Register

Beim Registrieren muss die Email-Adresse und das Passwort einem vorgegebenen Muster entsprechen. Ansonsten wird ein Hinweiß für den Nutzer angezeigt. Nach erfolgreichen Registrierung wird der Nutzer mit einem INSERT Query in der Datenbank hinzugefügt. 

<img src="./Screenshots/Registrieren.png" alt="Bildbeschreibung" style="width: 200px; height: auto;">


# Home

Auf der Home Activity werden alle verfügbaren Karten groß untereinander angezeigt.
Es ist möglich mit der Filterfunktion direkt nach Karten vom Typ "Banking", "Auto" oder "Gesundheit" zu suchen. Es ist auch möglich mit der "Suchen" Funktion nach beliebigen Karten zu suchen.

Oben links mit den "drei Strichen"-Button ist es möglich die Filterfunktions-Buttons ein oder auszublenedn.
Auch mit diesem Button kann man die Text-Filterung zurücksetzen.

Oben rechts mit dem Zahnrad (Einstellungs) -Button ist es möglich zu der Einstellungen-Activity zu kommen.

Unten rechts mit dem "Hinzufügen"-Button ist es möglich zu der Activity "Add Card Selection" zu kommen.

Es ist möglich auf eine beliebige Karte in der Liste zu klicken. Dann wir zu einer Detailansicht der Karte gewechselt.

<img src="./Screenshots/Home.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">


# Settings

In den Einstellungen ist es möglich sich auszuloggen. Nach dem Ausloggen wird automatisch zu der Anmelden-Activity gewechselt.

<img src="./Screenshots/Settings.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">


# Card Detail View

Hier wird eine Karte im Detail angezeigt. Je nach Kartentyp werden unterschiedliche Inhalte angezeigt.
Sobald der Button "NFC Aktivieren" gedrückt wird, simuliert das Handy die angezeigte Karte. Somit ist es möglich das Handy wie eine Karte zu verwenden, um zum Beispiel von einem NFC-Reader zum Bezahlen genutzt werden zu können. 
Mit dem erneuten Klicken auf den Button (Jetzt "NFC Deaktivieren") wir diese Funktion wieder beendet.
Nach dem Klicken des X-Buttons wird wieder zur Home Activity gewechselt


# Add Card Selection

Auf diesem Activity kann der Benutzer auswählen wie er eine neue Karte hinzufügen möchte.
1. Oben mit Kamera. Kann man Karten einfach hinzufügen in dem man ein Foto von der Karte macht. Das hilft dabei das der User die Daten nicht händisch übertragen muss.
2. Unten mit NFC. Das ist der Sichere Weg. Welcher zwingend für zum Beispiel einen Personalausweis oder eine Bankkarte notwendig ist.

<img src="./Screenshots/addCardSelection.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">


# Add Card Camera

Hier steht kurz geschrieben wir der Nutzer ein Foto von seine Karte machen soll.
Mit dem Button "Kamera öffnen" kommt er zu Kamera.

<img src="./Screenshots/addCardCameraBack.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">

# Take Photo

Hier ist es möglich ein Foto von der Karte zu machen.
Wenn Foto aufgenommen wird der Benutzer zu "Confirm Photo" weitergeleitet.

# Confirm Photo

Bei Confirm Photo kann der Benutzer das aufgenommene Foto bestägien oder zurück gehen um ein neues Foto aufzunehmen.
Wenn bestätigt wird man zur Activity "Card View To Save" weitergeleitet.

# Card View To Save (Photo)

Auf dieser Activity kann der User die Daten der Karte überprüfen.
Und nach Bedarf Anpassungen vornehmen, falls die erkannten Daten von der Kamera nicht richtig sind.
Dann kann der Benutzer auf "Speichern" klicken. Und gelangt zurück zur "Home" Activity, welche unten in der Recyclerview die gespeicherte Karte anzeigt.


# NFC Ready to Read

Screen mit Text "Bereit zum Lesen. Bitte halten Sie ihre Karte an die Rückseite ihres Smartphones." Sobald eine NFC-fähige Karte erkannt wird, wird zum "NFC Reading"-Screen gewechselt.  
<img src="./Screenshots/nfcReadyToRead.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">


# NFC Reading

Screen mit Wartesymbol bis das Auslesen abgeschlossen ist.
<img src="./Screenshots/nfcReading.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">


# Card View To Save (NFC)

Diese Activity ist wie die "Card View To Save (Photo)" nur dass die Felder der Daten nicht bearbeitbar sind, weil alle ausgelesenen Daten nicht verändert werden dürfen.

<img src="./Screenshots/cardViewToSave.png" alt="Bildbeschreibung" style="width: 20%; height: 20%;">
