---
icon: gamepad-modern
coverY: 0
---

# Abschlussprojekt

## Zufallsspiel mit Zahlen&#x20;

***

### Schritt 1: Module importieren

Wir brauchen das Modul `random` für Zufallszahlen und `time`, um Pausen einzubauen.

{% code overflow="wrap" %}
```
pythonKopierenBearbeitenimport randomimport time
```
{% endcode %}

***

### Schritt 2: Spielbegrüßung und Regeln anzeigen

Begrüße den Spieler und erkläre kurz die Spielregeln.

```
pythonKopierenBearbeitenprint("Willkommen zum Zufallsspiel!")print("Du hast 5 Versuche, eine Zahl zwischen 1 und 10 zu erraten.")print("Für jeden richtigen Tipp bekommst du einen Punkt.")print("Viel Erfolg!")
time.sleep(2)  # Kurze Pause von 2 Sekunden 
```

***

### Schritt 3: Punkte und Versuche initialisieren

Setze die Punkte und maximale Versuche auf 0 bzw. 5.

```
pythonKopierenBearbeitenpunkte = 0max_versuche = 5 
```

***

### Schritt 4: Schleife für Versuche starten

Erstelle eine Schleife, die für jeden Versuch einmal durchläuft.

```
pythonKopierenBearbeitenfor versuch in range(1, max_versuche + 1):
    print(f"\nVersuch {versuch} von {max_versuche}")
```

***

### Schritt 5: Zufallszahl erzeugen

Erzeuge für jeden Versuch eine neue Zufallszahl zwischen 1 und 10.

```
pythonKopierenBearbeiten    zahl = random.randint(1, 10)
```

***

### Schritt 6: Spieler nach Eingabe fragen und prüfen

Fordere den Spieler auf, eine Zahl einzugeben. Prüfe, ob die Eingabe gültig ist (Zahl zwischen 1 und 10).

```
pythonKopierenBearbeiten    while True:
        try:
            tipp = int(input("Rate eine Zahl zwischen 1 und 10: "))
            if 1 <= tipp <= 10:
                breakelse:
                print("Bitte gib eine Zahl zwischen 1 und 10 ein.")
        except ValueError:
            print("Das war keine gültige Zahl. Versuch es nochmal.")
```

***

### Schritt 7: Tipp mit Zufallszahl vergleichen

Wenn der Tipp richtig ist, Punkte erhöhen und Erfolg melden.

```
pythonKopierenBearbeiten    if tipp == zahl:
        print("Richtig! Du bekommst einen Punkt.")
        punkte += 1else:
        print(f"Falsch! Die richtige Zahl war {zahl}.")
```

***

### Schritt 8: Kurze Pause einbauen

Damit das Spiel nicht zu schnell ist, füge eine kurze Pause von 1 Sekunde ein.

```
pythonKopierenBearbeiten    time.sleep(1)
```

***

### Schritt 9: Punkte nach jedem Versuch anzeigen

Zeige nach jedem Versuch den aktuellen Punktestand.

```
pythonKopierenBearbeiten    print(f"Deine Punkte: {punkte}")
```

***

### Schritt 10: Spiel beenden und Gesamtergebnis ausgeben

Nach der Schleife gebe das Endergebnis aus und verabschiede den Spieler.

```
pythonKopierenBearbeitenprint("\nSpiel beendet!")print(f"Du hast {punkte} von {max_versuche} Punkten erreicht. Gut gemacht!")
```

***

## Komplett-Code (mit allen 10 Schritten)

```
pythonKopierenBearbeitenimport randomimport time
print("Willkommen zum Zufallsspiel!")print("Du hast 5 Versuche, eine Zahl zwischen 1 und 10 zu erraten.")print("Für jeden richtigen Tipp bekommst du einen Punkt.")print("Viel Erfolg!")
time.sleep(2)

punkte = 0max_versuche = 5for versuch in range(1, max_versuche + 1):
    print(f"\nVersuch {versuch} von {max_versuche}")
    zahl = random.randint(1, 10)

    while True:
        try:
            tipp = int(input("Rate eine Zahl zwischen 1 und 10: "))
            if 1 <= tipp <= 10:
                breakelse:
                print("Bitte gib eine Zahl zwischen 1 und 10 ein.")
        except ValueError:
            print("Das war keine gültige Zahl. Versuch es nochmal.")

    if tipp == zahl:
        print("Richtig! Du bekommst einen Punkt.")
        punkte += 1else:
```
