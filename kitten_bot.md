# Lernjournal: Mein Kitten Bot im verteilten Exploding-Kittens-Turnier

## Kurzbeschrieb

In diesem Projekt hab ich einen Bot namens **Lazy_Duck_Slayer_of_cyberjesus** gebaut, der in einem verteilten System das Spiel *Exploding Kittens* gegen die Bots meiner Klassenkameraden gespielt hat. Die Kommunikation lief über einen **Clowder Service** (quasi ein Discovery Service) und einem **Arena Service**, der die Spielrunden durchführte. Als Techstack hab ich **Python** und **WebSockets** verwendet. Ziel war’s, dass sich der Bot automatisch im System anmeldet, mit anderen Bots interagiert und in mehreren rundenbasierten Spielen möglichst lange überlebt – oder besser gesagt: gewinnt.

## Lernerfolge

- **Verständnis für verteilte Systeme**: Ich hab viel darüber gelernt, wie die Kommunikation zwischen verschiedenen Diensten funktioniert, besonders im Kontext von Discovery Services (Clowder) und Arena Services. Wie man Verbindungen stabil hält und gleichzeitig viele Instanzen von Bots verwaltet.

- **Umgang mit Websockets**: Beim Implementieren der Verbindungslogik mit WebSockets konnte ich meine Fähigkeiten in Python ausbauen. Die Kommunikation zwischen den Bots und dem Server war am Anfang tricky, aber mit etwas Geduld konnte ich alles zum Laufen bringen.

- **Bots & Spielelogik**: Ich hab gelernt, wie man einen Bot für ein rundenbasiertes Spiel programmiert. Es war spannend zu sehen, wie mein Bot interagiert, und noch spannender, wie er im Wettbewerb abschneidet.

- **Fehlerbehebung und Debugging**: Ich hab einige Bugs beseitigt, wie z.B. dass der Bot `NONE` zurückgab, anstatt `NoneType` zu benutzen. Solche kleinen Fehler können grossen Einfluss haben, und das Debuggen hat meine Problemlösungsfähigkeiten geschärft.

## Lernstrategie

Meine Lernstrategie war ziemlich unkompliziert – **Confidence is key**. Ich habe einfach den Plan verfolgt, den Bot zu programmieren, und mir keine grossen Gedanken darüber gemacht, was andere Bots tun oder wie das Spiel genau läuft. Die Idee war, dass mein Bot trotzdem immer eine Chance hat, zu gewinnen, egal was passiert. Ich hab mich auf die **Verbindung und Kommunikationslogik** konzentriert, und dann den Bot Schritt für Schritt implementiert. Als ich auf Probleme stiess, wie z.B. Verbindungsabbrüche, ging ich mit **Trial and Error** vor, bis ich eine Lösung gefunden habe.

## Fazit

Am Ende hat der Bot alle Erwartungen übertroffen – **über 200 Runden**, im Schnitt den **1. Platz** belegt und somit das Turnier gewonnen! Klar gab es noch ein paar Bugs zu fixen, aber die Erfahrung, meinen Bot im **Exploding-Kittens-Turnier** gegen die anderen zu sehen und zu testen, war ziemlich spannend. Nächstes Mal patch ich noch die kleinen Bugs und feile an der Logik, aber das Gefühl, gewonnen zu haben, war trotzdem sehr cool.

---

