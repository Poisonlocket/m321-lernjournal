# Lernjournal – LU02b: Vertikale und horizontale Verteilung

## Kurzbeschrieb
Im Theorieblock LU02b behandelten wir die Themen **vertikale und horizontale Verteilung** in verteilten Systemen. Dabei ging es darum, wie Aufgaben und Ressourcen innerhalb eines Systems organisiert und verteilt werden können. Die vertikale Verteilung beschreibt die Aufteilung von Aufgaben auf verschiedene Schichten oder Ebenen (z.B. Präsentations-, Anwendungs- und Datenbankschicht), während die horizontale Verteilung die Vervielfältigung gleicher Komponenten über mehrere Knoten hinweg meint. Wir haben uns angeschaut, wie diese beiden Konzepte in realen Systemen kombiniert eingesetzt werden können. Unser Beispiel war die schweizer Post, ahand welcher wir aufgezeigt haben wie ein verteiltes System funktioniert.

## Lernerfolge
Ich habe durch diesen Block ein besseres Verständnis dafür gewonnen, **wann und warum** man Systeme vertikal oder horizontal verteilt. Besonders wichtig fand ich die Unterscheidung zwischen **horizontaler und vertikaler Skalierung**, die jeweils unterschiedliche Anforderungen und Herausforderungen mit sich bringen. Ich konnte mir durch die Beispiele (z.B. Webshop und SETI@home) gut vorstellen, wie solche Architekturen in der Praxis aussehen. Zusätzlich habe ich gelernt, dass hybride Ansätze oft notwendig sind, um die Vorteile beider Methoden zu kombinieren.

## Lernstrategie
Ich bin beim Lernen so vorgegangen, dass ich die wichtigsten Begriffe und Konzepte während dem Unterricht **stichwortartig notiert** und anschliessend mit eigenen Worten zusammengefasst habe. Das hilft mir, die Inhalte besser aufzunehmen. Das Erarbeiten von Praxisbeispielen hat mir sehr geholfen, die Theorie greifbar zu machen.

## Fazit
Durch diesen Unterrichtsblock habe ich erkannt, wie entscheidend eine gute Systemarchitektur für die **Skalierbarkeit und Stabilität** von Anwendungen ist. Meine Lernstrategie mit eigenen Notizen hat sich als sehr effektiv erwiesen, und ich werde sie auch bei zukünftigen Theorieblöcken weiter anwenden. Für die nächsten Learning Units nehme ich mir vor, zusätzlich noch mehr auf **praktische Beispiele und Anwendungen** zu achten, um die Theorie noch besser mit der Realität verknüpfen zu können.

---
![skalierung image](./img/skalierung.jpg)
---

## 📘 Glossar


**Vertikale Skalierung**  
Leistungssteigerung eines **einzelnen Systems** durch Aufrüsten der Hardware (z.B. mehr RAM, stärkere CPU). Gut für einfache Verwaltung, aber begrenzt in der Erweiterbarkeit.

**Horizontale Skalierung**  
Erweiterung der Systemleistung durch **Hinzufügen zusätzlicher Instanzen** oder Server. Bietet bessere Skalierbarkeit und Ausfallsicherheit.

**Verteiltes System**  
Ein System, das aus mehreren **miteinander verbundenen, eigenständigen Computern** besteht, die zusammenarbeiten, um eine gemeinsame Aufgabe zu erfüllen.

**Hybrid-Skalierung**  
Kombination aus vertikaler und horizontaler Skalierung, um die Vorteile beider Methoden zu nutzen – häufig in komplexen Systemarchitekturen eingesetzt.

**Loadbalancing**  
Die gleichmässige Verteilung von Traffic auf mehrere Nodes, um Überlastungen zu vermeiden und die Leistung zu optimieren.

**Ausfallsicherheit**  
Fähigkeit eines Systems, **trotz Fehlern oder Ausfällen einzelner Komponenten** weiterhin zuverlässig zu funktionieren. -> Replica Funktion in Docker Stack



