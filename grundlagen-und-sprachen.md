# Vergleich: Python vs. JavaScript – Grundlagen der Programmierung

Wenn man Programmieren lernt, begegnet man schnell den Sprachen **Python** und **JavaScript**. Beide sind sehr beliebt, aber sie unterscheiden sich in ihrer Denkweise, Syntax und Anwendung. Wer die Unterschiede versteht, lernt gleichzeitig viele grundlegende Programmierkonzepte.

---

##  Ziel und Einsatzgebiete

| Sprache       | Hauptanwendung                           |
|---------------|-------------------------------------------|
| **Python**    | Datenanalyse, Automatisierung, Bildung, KI, Web-Backends |
| **JavaScript**| Webentwicklung (Front-End und zunehmend auch Back-End mit Node.js) |

---

##  Syntax: Klarheit vs. Flexibilität

### Python

Python wurde mit dem Ziel entwickelt, **einfach lesbar und logisch aufgebaut** zu sein. Es verwendet **Einrückungen** statt Klammern, um Blöcke zu strukturieren.

```python
# Python
x = 5
if x > 3:
    print("Grösser als 3")
```
JavaScript nutzt geschweifte Klammern {} zur Strukturierung und ist flexibler, aber dadurch oft schwerer zu lesen für Einsteiger:innen.
````
// JavaScript
let x = 5;
if (x > 3) {
    console.log("Grösser als 3");
}
`````
Python: Dynamisch und lesbar
````
name = "Eliza"     # String
alter = 17         # Integer
aktiv = True       # Boolean
liste = [1, 2, 3]  # Liste (mutable)
````
JavaScript: Dynamisch, aber mit Eigenheiten
````
let name = "Eliza";     // String
let alter = 17;         // Number
let aktiv = true;       // Boolean
let liste = [1, 2, 3];  // Array (mutable)
````
In beiden Sprachen muss man keinen Datentyp explizit angeben – das macht sie dynamisch typisiert. JavaScript ist dabei etwas ungenauer (z. B. bei null, undefined, NaN).

## Schleifen und Bedingungen
Python
````
for zahl in [1, 2, 3]:
    print(zahl)
````
JavaScript
````
for (let zahl of [1, 2, 3]) {
    console.log(zahl);
}
````

## Objekte & Dictionaries
Python: Dictionary
````
person = {
    "name": "Eliza",
    "alter": 17
}
print(person["name"])
````
JavaScript: Objekt
````
let person = {
    name: "Eliza",
    alter: 17
};
console.log(person.name);
`````
## Fehlerbehandlung
Python
Python stoppt bei Fehlern sofort und zeigt klare Fehlermeldungen:
````
zahl = int("abc")  # Fehler: ungültige Zahl
````
JavaScript
JavaScript läuft manchmal weiter, obwohl ein Fehler vorliegt – das kann zu versteckten Bugs führen:
````
let zahl = parseInt("abc"); // Ergebnis: NaN (kein Fehler)
````

## Objektorientierung
Python nutzt klassische Klassen wie in Java oder C++:
````
class Katze:
    def __init__(self, name):
        self.name = name
````
JavaScript basiert auf Prototypen, unterstützt aber auch Klassen (seit ES6):
````
class Katze {
    constructor(name) {
        this.name = name;
    }
}
````
| Thema                   | Python                        | JavaScript                            |
| ----------------------- | ----------------------------- | ------------------------------------- |
| Syntax                  | Sehr leserfreundlich          | Etwas komplexer, flexibler            |
| Einstieg                | Ideal für Anfänger\:innen     | Auch möglich, aber teils verwirrend   |
| Fehlerbehandlung        | Klar und direkt               | Lässt Fehler manchmal „durchrutschen“ |
| Webentwicklung          | Nur im Backend (z. B. Django) | Frontend und Backend (z. B. Node.js)  |
| Automatisierung/Skripte | Sehr gut geeignet             | Weniger verbreitet                    |
| Datenanalyse/KI         | Python ist führend            | Kaum genutzt                          |

