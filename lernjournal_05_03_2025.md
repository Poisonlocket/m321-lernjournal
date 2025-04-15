# Lernjournal LU07a – LU08d: Discovery und Gateway Services

## Kurzbeschrieb

In diesen Lektionen haben wir zwei zentrale Begriffe aus der Welt der verteilten Systeme angeschaut: **Discovery Services** und **Gateway Services**. Beide sind wichtige Bestandteile moderner Architekturen mit Microservices und tragen wesentlich dazu bei, dass solche Systeme **skalierbar**, **zuverlässig** und **flexibel** bleiben.

## Grundlagen Discovery Service

Ein **Discovery Service** sorgt dafür, dass sich verschiedene Services in einem System gegenseitig finden und miteinander kommunizieren können, auch wenn sich ihre IP-Adressen oder Standorte ständig ändern. Das ist vor allem in dynamischen Umgebungen wichtig, wie man sie in der Cloud oft hat.

### Aufgaben eines Discovery Services:

- **Registrierung**: Ein Service meldet sich beim Discovery Service an und gibt an, wo er erreichbar ist (IP, Port etc.).
- **Service-Entdeckung**: Andere Services können beim Discovery Service nachfragen, wo sich ein gewünschter Dienst befindet.
- **Dynamische Updates**: Neue Instanzen können automatisch erkannt werden.
- **Fehlerbehandlung**: Wenn ein Service ausfällt, wird er aus dem Register entfernt.

Ein bekanntes Beispiel dafür ist **Netflix Eureka** – ein Open-Source-Tool zur Verwaltung von Microservices.


## Grundlagen Gateway Service

Ein **Gateway Service** ist der zentrale Einstiegspunkt für die Kommunikation zwischen einem Client (z.B. ein Browser oder eine Mobile App) und den verschiedenen internen Services eines Systems.

### Funktionen eines Gateway Services:

- **Routing und Weiterleitung**: Weiterleitung von Anfragen an den richtigen Service, je nach URL oder Methode.
- **Transformation**: Konvertierung von Daten in ein einheitliches Format, z.B. JSON.
- **Aggregation**: Zusammenfassen von Antworten mehrerer Services zu einer.
- **Authentifizierung und Autorisierung**: Prüfen von Benutzerrechten mittels z.B. JSON Web Tokens.
- **Lastverteilung**: Gleichmässiges Verteilen der Anfragen auf verschiedene Instanzen.
- **Protokollierung und Überwachung**: Logging und Sammeln von Metriken zur Systemüberwachung.



Der Gateway übernimmt auch die Aufgabe, **Anfragen zu formatieren** und **Antworten zusammenzustellen**, damit der Client nur mit einer klaren API sprechen muss.

## Unterschiede zwischen Gateway und Discovery

| Merkmal | Gateway Service | Discovery Service |
|--------|------------------|----------------|
| **Zweck** | Schnittstelle zwischen Clients und Services | Verwaltung der Erreichbarkeit von Services |
| **Hauptaufgabe** | Anfragevermittlung, Sicherheit, Logging | Registrierung & Lokalisierung von Services |
| **Wer spricht mit wem?** | Client → Gateway → Service | Service ↔ Discovery ↔ Service |
| **Beispiel** | API-Gateway für Online-Shop | Netflix Eureka |

### Zusammenfassung
Man kann sagen:
- Der **Gateway Service** ist zuständig für die Kommunikation **von aussen nach innen** (Client → System).
- Der **Discovery Service** sorgt dafür, dass die Services **untereinander** wissen, wo sie sich befinden.

## Lernerfolge

Ich habe verstanden, wie Microservices so miteinander verbunden werden können, dass sie auch in komplexen oder verteilten Systemen zuverlässig funktionieren. Besonders wichtig war für mich das Prinzip der **dynamischen Service-Entdeckung**, bei dem sich neue Dienste automatisch registrieren und auffindbar werden – das spart Zeit und reduziert Konfigurationsaufwand.

Beim **Gateway Service** habe ich gelernt, wie man eingehende Anfragen **bündelt**, **weiterleitet** und **prüft**, das alles an einem zentralen Ort. Dadurch kann man die internen Services sauber kapseln und trotzdem von aussen einfach darauf zugreifen.

Ich weiss jetzt, dass diese beiden Dienste oft **Hand in Hand** arbeiten und zusammen die Grundlage für eine **skalierbare**, **sichere** und **wartbare** Systemarchitektur bilden.

## Lernstrategie

Ich bin so vorgegangen, dass ich zuerst die theoretischen Grundlagen im Unterricht aufgenommen habe. Danach habe ich mir konkrete Beispiele wie **Netflix Eureka** und ein E-Commerce-System angeschaut, um das Ganze besser zu verstehen. Die Visualisierungen und das Aufzeichnen von Abläufen in Skizzen haben mir geholfen, den Überblick zu behalten.

Zusätzlich habe ich weiterführende Artikel gelesen, z.B. von Heise und Datacenter Insider, um ein besseres Bild davon zu bekommen, wie diese Konzepte in der Praxis eingesetzt werden. Dabei habe ich mich auf die Funktionsweise konzentriert, statt auf die konkrete Implementierung in einem bestimmten Framework.



## Glossar

- **Discovery Service**: Vermittler zwischen Services, der Adressen & Verfügbarkeiten verwaltet.
- **Gateway Service**: Zentrale Schnittstelle für Anfragen von Clients.
- **Routing**: Entscheidung, welche Anfrage wohin geht.
- **Netflix Eureka**: Discovery-Service von Netflix, FOSS.

## Bongo Cat Counter
Für dieses Lernjournal wurden 6069 Bongo Cat Taps verwendet, meinem [Bongo Kätzchen](https://store.steampowered.com/app/3419430/Bongo_Cat/) Bluten die Pfötchen.