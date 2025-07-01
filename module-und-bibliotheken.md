# Module & Bibliotheken

In Python gibt es mehrere eingebaute Module, die dir bei mathematischen Operationen, Zufallszahlen und Zeitmessung helfen. Diese sind besonders nützlich, wenn du Programme schreiben willst, die z.B. Berechnungen durchführen, Zufallswerte erzeugen oder Zeitabläufe steuern.

---

##  Mathematische Funktionen mit `math`

Das Modul `math` bietet viele nützliche Funktionen für mathematische Berechnungen:

```python
import math

print(math.sqrt(16))    # Quadratwurzel: 4.0
print(math.pi)          # Wert von Pi: 3.141592653589793
print(math.sin(math.pi / 2))  # Sinus von 90 Grad (Pi/2): 1.0
````
math.sqrt(x) — Quadratwurzel von x
math.sin(x), math.cos(x), math.tan(x) — trigonometrische Funktionen
math.ceil(x) — Aufrunden
math.floor(x) — Abrunden
math.factorial(n) — Fakultät von n

## Zufallszahlen mit random
Das random-Modul ermöglicht das Erzeugen von Pseudo-Zufallszahlen.
````
import random

print(random.random())        # Zufallszahl zwischen 0 und 1
print(random.randint(1, 10))  # Zufallszahl zwischen 1 und 10 (inklusive)
print(random.choice(['A', 'B', 'C']))  # Zufällige Auswahl aus einer Liste
````
## Nützliche Funktionen
random.random() — float zwischen 0.0 und 1.0
random.randint(a, b) — ganze Zahl zwischen a und b
random.choice(seq) — zufälliges Element aus Sequenz
random.shuffle(list) — mischt die Reihenfolge einer Liste

## Zeitfunktionen mit time
Mit dem time-Modul kannst du Zeiten messen oder Pausen in Programmen einbauen.
````
import time

print(time.time())        # Aktuelle Zeit in Sekunden seit 1970 (Unix-Zeit)
time.sleep(2)             # Programm pausiert 2 Sekunden
print("2 Sekunden sind vergangen")
````

## Wichtige Funktionen
time.time() — aktuelle Zeit als Unix-Timestamp
time.sleep(sekunden) — pausiert das Programm für angegebene Sekunden
time.localtime() — aktuelle lokale Zeit als Struktur

