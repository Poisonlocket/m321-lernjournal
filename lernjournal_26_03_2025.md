# Lernjournal: Verteilte Datenhaltung und Apache Cassandra

## Kurzbeschrieb
In diesem Unterrichtsblock ging’s um die Grundlagen der verteilten Datenhaltung. Ich hab gelernt, wie man Daten über mehrere Rechner verteilt speichert, um die Last besser zu verteilen und wie man so die Skalierbarkeit erhöht. Wir haben auch gelernt, wie Replikation und Partitionierung funktionieren und welche Techniken dafür verwendet werden. Danach haben wir das Ganze mit einer praktischen Analyse von Apache Cassandra vertieft.

## Lernerfolge
- **Verteilte Datenhaltung**: Ich habe verstanden, wie Daten über mehrere Knoten in einem System verteilt werden können und was Replikation und Partitionierung damit zu tun haben.
- **Skalierbarkeit**: Wir haben herausgefunden, wie man die Skalierbarkeit eines Systems verbessert, indem man die Daten auf mehrere Server aufteilt und Anfragen verteilt.
- **Cassandra**: Ich konnte die wichtigsten Features von Cassandra lernen, wie etwa die Replikation und Partitionierung, und wie es mit grossen Datenmengen umgehen kann.

## Lernstrategie
Ich habe den Artikel durchgelesen, die Konzepte und Beispiele analysiert und mir die wichtigsten Punkte notiert. Besonders bei den praktischen Beispielen habe ich viel Wert darauf gelegt, die Replikations- und Partitionierungsstrategien zu verstehen und mir zu merken, welche Optionen Cassandra da bietet. Danach hab ich die Theorie mit der Analyse von Cassandra verknüpft, um zu sehen, wie die Theorie in der Praxis angewendet wird.

## Fazit
Ich habe viel über die Grundlagen der Datenhaltung gelernt und wie das Ganze bei verteilten Systemen wie Cassandra funktioniert. Das Wissen über Replikation, Partitionierung und Konsistenz wird mir sicher in zukünftigen Projekten helfen, besonders wenn’s um Systeme mit vielen Daten geht. Die Analyse von Cassandra hat mir auch gezeigt, wie man mit grossen Datenmengen und hohen Zugriffszahlen umgehen kann. Wenn ich in Zukunft ein System aufbaue, das solche Anforderungen hat, könnte Cassandra echt eine gute Wahl sein.

---

## 📚 Glossar

**Verteilte Datenhaltung**: Die Speicherung von Daten auf mehreren Knoten oder Rechnern eines Netzwerks, um Skalierbarkeit, Verfügbarkeit und Ausfallsicherheit zu erhöhen.

**Replikation**: Das Anlegen von Kopien derselben Daten auf mehreren Knoten eines Systems, um bei einem Ausfall weiterhin auf die Daten zugreifen zu können.

**Partitionierung**: Die Aufteilung von grossen Datenmengen in kleinere Einheiten, die auf unterschiedlichen Knoten gespeichert werden. Dadurch wird die Last gleichmässiger verteilt.

**ACID**: Ein Konzept aus der klassischen Datenbanktheorie, das für Transaktionen steht, die atomar, konsistent, isoliert und dauerhaft sein müssen.

**BASE**: Ein alternatives Modell zu ACID, das bei verteilten Systemen häufiger eingesetzt wird. Es steht für „Basically Available, Soft State, Eventually Consistent“.

**Eventual Consistency**: Ein Konsistenzmodell, bei dem sichergestellt ist, dass alle Kopien der Daten irgendwann denselben Stand haben – aber nicht notwendigerweise sofort.

**Consistent Hashing**: Ein Verfahren zur Partitionierung von Daten, das besonders gut mit dynamisch wechselnden Knotenanzahlen umgehen kann.

**QUORUM**: Ein Konsistenzlevel bei Cassandra, bei dem eine Mehrheit der Knoten antworten muss, um eine Lese- oder Schreiboperation als erfolgreich zu bewerten.

**Cassandra**: Eine verteilte NoSQL-Datenbank, die für hohe Verfügbarkeit, horizontale Skalierbarkeit und schnelle Verarbeitung grosser Datenmengen entwickelt wurde.

**NoSQL**: Eine Klasse von Datenbanken, die nicht auf relationalen Modellen basiert. Sie sind meist schemalos, horizontal skalierbar und besonders geeignet für grosse, verteilte Systeme.

## Bongo Cat Counter
Für dieses Lernjournal wurden 4632 Bongo Cat Taps verwendet, mein [Bongo Kätzchen](https://store.steampowered.com/app/3419430/Bongo_Cat/) ist vom Streik zurückgekehrt und trommelt fleissig weiter. <br>
![Bongo Cat](./img/Bongo_cat.png)