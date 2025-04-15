# Lernjournal – Pub/Sub und MQTT

## Kurzbeschrieb
In diesem Unterrichtsblock haben wir das Kommunikationsmodell **Publish/Subscribe (Pub/Sub)** kennengelernt, das insbesondere im Kontext vom **Internet of Things (IoT)** eine zentrale Rolle spielt. Im Fokus standen die Konzepte hinter Pub/Sub, die beteiligten Komponenten (Publisher, Subscriber, Pub/Sub-System) sowie das leichtgewichtige Protokoll **MQTT**, das dieses Modell in der Praxis umsetzt. Ein besonderes Augenmerk lag auf den Vorteilen der Entkopplung, Skalierbarkeit und Zuverlässigkeit solcher Systeme. Anhand eines Hausautomationsbeispiels wurde aufgezeigt, wie solche Systeme in der Realität funktionieren können.

## Lernerfolge
Ich konnte mir einen klaren Überblick über die Funktionsweise von Pub/Sub-Systemen verschaffen. Es wurde mir bewusst, wie wichtig die Entkopplung von Publishern und Subscribern ist, um flexible und skalierbare Systeme zu entwickeln. Besonders spannend fand ich das MQTT-Protokoll, das genau für solche Anforderungen im IoT-Bereich entwickelt wurde. Ich kenne jetzt, was die verschiedenen **QoS-Stufen (Quality of Service)** bedeuten und wie sie sich auf die Nachrichtenzustellung auswirken. Ausserdem wurde mir der Nutzen von Themenstrukturen (z.B. Küche/Kühlschrank/Temperatur) und retained messages klar.

## Lernstrategie
Meine Strategie war, den empfohlenen Artikel von der Website der Firma EMQX aufmerksam zu lesen. Dabei habe ich mir beim Lesen Notizen gemacht, die wichtigsten Begriffe markiert und das Beispiel mit Publisher und Subscriber in Python nachverfolgt. Um das Ganze besser zu verstehen, habe ich versucht, die Erklärungen in eigenen Worten zusammenzufassen. Dabei habe ich insbesondere darauf geachtet, die Begriffe wie „Thema“, „Broker“ oder „QoS“ richtig einzuordnen. Zudem habe ich auf Moodle nochmal die Theorie aus den vorherigen Wochen zu Pub/Sub durchgelesen – das hat mir beim Einordnen des neuen Stoffs sehr geholfen.

## Fazit
Obwohl die Thematik auf den ersten Blick technisch wirkt, ist sie logisch aufgebaut und nachvollziehbar. Die Beispiele und das klare Kommunikationsmodell haben mir geholfen, das Ganze besser zu verstehen. In Zukunft möchte ich MQTT selbst mal ausprobieren und deployen – zum Beispiel in einem kleinen Raspberry-Pi oder ESP32 Webserver zu Hause. Durch das strukturierte Lesen und Zusammenfassen kann ich mir neue Inhalte gut erarbeiten – diese Strategie möchte ich beibehalten.

## Beispiel
Ein einfaches Beispiel eines solchen Pub/Sub Services ist [NTFY](https://ntfy.sh) welchen ich auch selbst als Docker Container verwende und betreibe.

## Glossar

**Pub/Sub (Publish/Subscribe)**  
Ein Kommunikationsmodell, bei dem Nachrichten von Publishern an ein zentrales System gesendet werden und von dort an alle abonnierten Subscriber verteilt werden. Publisher und Subscriber kennen sich nicht direkt.

**Publisher**  
Ein System oder Gerät, das Nachrichten erzeugt und an das Pub/Sub-System sendet.

**Subscriber**  
Ein System oder Gerät, das sich für bestimmte Themen registriert, um passende Nachrichten vom Pub/Sub-System zu empfangen.

**Pub/Sub-System / Broker**  
Die vermittelnde Instanz, die Nachrichten von Publishern entgegennimmt und an alle passenden Subscriber verteilt. In MQTT nennt man diesen Vermittler „Broker“.

**MQTT (Message Queuing Telemetry Transport)**  
Ein leichtgewichtiges Protokoll, das auf dem Pub/Sub-Modell basiert und speziell für Geräte mit wenig Ressourcen (z.B. im IoT-Bereich) entwickelt wurde.

**Thema (Topic)**  
Ein logischer Kanal, über den Nachrichten organisiert und verteilt werden. Topics können hierarchisch strukturiert sein (z.B. `huus/stube/liecht`).

**Nachricht**  
Die Daten, die ein Publisher sendet und ein Subscriber empfängt. Kann z.B. ein Temperaturwert, ein Ereignis oder ein Text sein.

**QoS (Quality of Service)**  
Die Stufe der Zuverlässigkeit bei der Zustellung einer Nachricht. MQTT kennt drei QoS-Stufen:
- **0**: At most once – Nachricht wird einmal gesendet, ohne Bestätigung.
- **1**: At least once – Nachricht wird so lange gesendet, bis sie bestätigt wurde.
- **2**: Exactly once – Nachricht wird genau einmal empfangen, auch bei Verbindungsproblemen.

**Retained Message**  
Eine vom Broker gespeicherte Nachricht, die automatisch an neue Subscriber gesendet wird, sobald sie sich für ein Thema anmelden.

**Entkopplung**  
Das Prinzip, dass Sender und Empfänger von Nachrichten nicht voneinander wissen müssen. Das erhöht die Flexibilität und Wartbarkeit eines Systems.


## Bongo Cat Counter
Für dieses Lernjournal wurden 5485 Bongo Cat Taps verwendet, meine [Bongo Kätzchen](https://store.steampowered.com/app/3419430/Bongo_Cat/) macht mittlerweile Gebrauch vom Streikrecht.