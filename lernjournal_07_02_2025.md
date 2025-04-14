# Lernjournal – RESTful Webservices, Flask-RESTful & AJAX


---

##  Kurzbeschrieb
In diesem Unterrichtsblock ging es um die Grundlagen von RESTful Webservices und deren praktische Umsetzung mit dem Python-Framework Flask-RESTful. Zudem wurde AJAX als Technik zur asynchronen Datenübertragung im Browser eingeführt. Ich habe gelernt, wie man eine REST-API erstellt, wie man Anfragen strukturiert und verarbeitet, und wie man mit `fetch()` Daten vom Server laden kann, ohne die Seite neu zu laden.

---

##  Lernerfolge

- Ich verstehe nun, was einen RESTful Webservice ausmacht: Ressourcen, URI, HTTP Methoden (GET, POST, PUT, DELETE) und Statuscodes.
- Ich kann einfache APIs mit Flask-RESTful schreiben und weiss, wie ich Ressourcenklassen implementiere.
```python
class Bug(Resource):
    def get(self):
        if not bugs:
            return {"message": "Keine Bugs gefunden. Dein Code läuft... für jetzt."}, 200
        return {"bugs": bugs}, 200

    def post(self):
        bug_data = request.json
        bug_description = bug_data.get("description", "Unbekannter Bug")
        bugs.append(bug_description)
        return {
            "message": f"Bug gespeichert: '{bug_description}'. Glückwunsch, du hast gerade technische Schulden produziert!",
            "total_bugs": len(bugs)
        }, 201
```
- Ich kenne den Unterschied zwischen Query-Parametern (z.B. in der URL enthalten) und Formular-Parametern (z.B. im Body).
- Ich habe verstanden, wie `fetch()` funktioniert und wie es verwendet wird, um eine Textdatei dynamisch in eine Webseite zu laden.
- Ich kann die Bedeutung von Statuscodes wie `200 OK`, `404 Not Found` oder `500 Internal Server Error` einordnen und anwenden.

---

##  Lernstrategie

Ich habe den Unterricht aufmerksam verfolgt und mir Notizen gemacht. Besonders hilfreich war für mich das Schreiben eines eigenen kleinen Webservices in Flask mit einer `HelloWorld`-Ressource. Ich habe die Beispiele mit eigenen Parametern erweitert, um ein besseres Gefühl für den Datenfluss zu bekommen. Danach habe ich die AJAX-Beispiele Schritt für Schritt nachgebaut und verändert, um deren Funktionsweise zu verstehen. Ich habe auch viel mit Konsolenausgaben und `print()`-Statements gearbeitet, um zu sehen, wann welcher Teil des Codes aktiv ist (und vorallem weil ich den Debugger immer noch nicht wirklich effizient brauchen kann).

---

## Fazit

Durch die praktische Arbeit mit Flask-RESTful und AJAX habe ich ein besseres Verständnis für die Kommunikation zwischen Frontend und Backend bekommen ohne State speichern zu können.

---
![Restful Logo](./img/flask_restful.png)
---
## Glossar

- **REST**: Ein Architekturstil für Webservices, bei dem Ressourcen über HTTP eindeutig per URI angesprochen werden.
- **URI**: Eine eindeutige Adresse, unter der eine Ressource im Web erreichbar ist (z.B. `/api/user/1`).
- **HTTP-Methoden**: Befehle wie GET, POST, PUT und DELETE, mit denen Clients dem Server mitteilen, was sie tun möchten.
- **Statuscode**: Eine Antwort vom Server, die den Zustand der Anfrage beschreibt – z.B. `200 OK` für erfolgreich oder `404 Not Found` für eine nicht gefundene Ressource. Mein persönlicher Lieblingsstatuscode ist aber `503 Service Unavailable`, weil sich mein Gehirn aktuell genau so fühlt.
- **Query-Parameter**: Daten, die direkt in der URL übergeben werden, z.B. `/search?q=flask`.
- **Formular-Parameter**: Daten, die im Body einer POST-Anfrage übermittelt werden, z.B. bei einem Login-Formular.
- **AJAX**: Eine Technik, mit der Webanwendungen Daten im Hintergrund laden können, ohne die ganze Seite neu zu laden (Asynchroner Request auf ein Node JS Backend).
- **`fetch()`**: Eine moderne JavaScript-Funktion, mit der Daten asynchron vom Server angefordert werden können.
- **JSON**: Die Javascript Objekt Notation.


