---
icon: vector-circle
---

# Objektorientierte Programmierung

## Objektorientierte Programmierung Python

Die objektorientierte Programmierung (OOP) ist ein Programmierstil, bei dem man versucht, die Welt in **Objekte** und **Klassen** abzubilden.

Ein Objekt ist eine **Instanz einer Klasse** – also ein konkretes "Ding", das bestimmte Eigenschaften (Attribute) und Fähigkeiten (Methoden) hat.

***

### Klassen und Objekte

Eine **Klasse** ist wie ein Bauplan. Ein **Objekt** ist das, was nach dem Bauplan erschaffen wird.

Beispiel:

```python
class Hund:
    def bellen(self):
        print("Wuff!")
```



Hier wird die Klasse `Hund` definiert. Sie hat eine Methode mit dem Namen `bellen`.

Ein Objekt wird so erstellt:

```python
pythonKopierenBearbeitenmein_hund = Hund()
mein_hund.bellen()  # Ausgabe: Wuff!
```



### Die init()-Methode

Die Methode `__init__()` wird automatisch aufgerufen, wenn ein neues Objekt erstellt wird. Sie dient dazu, dem Objekt **Startwerte** mitzugeben – zum Beispiel Name oder Alter.

```python
pythonKopierenBearbeitenclass Hund:
    def __init__(self, name, alter):
        self.name = name
        self.alter = alter

    def vorstellen(self):
        print("Ich bin " + self.name + " und ich bin " + str(self.alter) + " Jahre alt.")
```

#### Erklärung:

* `__init__` wird beim Erstellen eines neuen Objekts automatisch ausgeführt.
* `self` ist ein Verweis auf das aktuelle Objekt.
* Die Parameter `name` und `alter` werden beim Erstellen übergeben.
* Diese Werte werden in den Objektvariablen `self.name` und `self.alter` gespeichert.

Beispiel für die Verwendung:

```python
pythonKopierenBearbeitenhund1 = Hund("Bello", 3)
hund2 = Hund("Luna", 5)

hund1.vorstellen()  # Ausgabe: Ich bin Bello und ich bin 3 Jahre alt.
hund2.vorstellen()  # Ausgabe: Ich bin Luna und ich bin 5 Jahre alt.
```

***

### Warum OOP?

Objektorientierte Programmierung hilft dabei, größere Programme besser zu strukturieren. Man kann:

* Daten und Funktionen logisch bündeln
* Wiederverwendbaren Code schreiben
* Dinge aus der realen Welt (wie Tiere, Autos, Personen) besser darstellen

***

### Begriffe im Überblick

| Begriff      | Bedeutung                                                                 |
| ------------ | ------------------------------------------------------------------------- |
| Klasse       | Ein Bauplan für Objekte                                                   |
| Objekt       | Ein konkretes Exemplar einer Klasse                                       |
| Attribut     | Eine Eigenschaft eines Objekts                                            |
| Methode      | Eine Funktion, die zu einem Objekt gehört                                 |
| `__init__()` | Eine Methode, die beim Erzeugen eines Objekts automatisch ausgeführt wird |
| self         | Verweist innerhalb der Klasse auf das aktuelle Objekt                     |
