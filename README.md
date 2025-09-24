# Fact-or-Fake — Wiki Game zur Faktenüberprüfung

**Fact-or-Fake** ist ein textbasiertes Quiz-/Bildungsspiel, bei dem Spieler zwischen echten und erfundenen Fakten (aus Wikipedia) unterscheiden müssen. Ziel ist es, spielerisch die Fähigkeit zur Quellenkritik und Faktenprüfung zu schärfen. Entstanden in einem Hackathon über 3 Tage.

---

## Inhaltsverzeichnis

1. [Features](#features)  
2. [Mein Beitrag](#mein-beitrag)  
3. [Installation](#installation)  
4. [Benutzung](#benutzung)  
5. [Projektstruktur](#projektstruktur)  
6. [Mitwirkende](#mitwirkende)  

---

## Features

- Auswahl von **Schwierigkeitsstufen** (z. B. einfach, mittel, schwer)  
- Echtzeit-Daten aus Wikipedia  
- interaktives Konsoleninterface  
- Mehrspieler-Modus für bis zu 5 Spieler  
- Punktesystem & Verlauf der Spielergebnisse  


---

## Mein Beitrag

Ich war hauptsächlich Verantwortlich für:

- **Scraping und Beschaffung der Fakten**: Automatisiertes Auslesen von Informationen aus Wikipedia bzw. verwandten Quellen, um wahr/falsch-Aussagen zu generieren.  
- **Manipulation / Generierung von Falschaussagen**: Erzeugung von synthetisch verfälschten Versionen echter Fakten, so dass sie glaubwürdig genug sind, aber dennoch falsch.  
- Integration dieser Fakten in die Quizlogik und Sicherstellung, dass beide Varianten (Fact und Fake) sinnvoll und ausgewogen sind.

---

## Installation

```bash
git clone https://github.com/Mk97x/Fact-or-Fake.git
cd Fact-or-Fake

# Virtuelle Umgebung (empfohlen)
python3 -m venv venv
source venv/bin/activate  # auf Windows ggf. venv\Scripts\activate

# Abhängigkeiten installieren
pip install -r requirements.txt
```

## Benutzung
```bash
python main.py
```
Wähle die Anzahl der Spieler (1-5)

Wähle eine Schwierigkeitsstufe

Pro Runde bekommst du zwei Aussagen – eine ist wahr, die andere falsch

Tippe ein, welche Aussage du für „Fake“ hältst

Punktevergabe: richtiger Tipp = +1 Punkt, falscher Tipp = kein Punkt 

## Projektstruktur
```bash
Fact-or-Fake/
├── main.py                  # zentrale Spiellogik & Einstiegspunkt
├── controller/
│   └── question_generator.py  # Logik zur Auswahl und Generierung der Faktenpaare
├── view/
│   └── game_gui.py             # Darstellung & Nutzerinterface (Konsole)
├── README.md
├── requirements.txt           # alle Python-Abhängigkeiten
```
## Mitwirkende

[**[Kristina Krauberger](https://github.com/kristina-krauberger)**] —  UI / Spielgestaltung / Management

[**[Marie Hirte](https://github.com/Its-Marie)**] —  UI / Spielgestaltung

[**[Fabio Morena](https://github.com/fabiomorena)**] - Web Scraping / Faktenmanipulation

[**[Enrico Harder](https://github.com/EnricoHarder)**] — Web Scraping / UI / Projektleiter

[**[Victor von Reiche](https://github.com/victor-von-reiche)**] - Spielgetstaltung / Präsentation

**[Jan Donath]** - Spielablauf

[**[Martin Koch](https://github.com/Mk97x)**] — Web Scraping / Faktenmanipulation 


