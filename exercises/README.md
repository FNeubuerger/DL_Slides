# Deep Learning Übungen - FH Südwestfalen

## Übersicht

Diese Sammlung enthält 5 umfassende Übungsblätter für die Deep Learning Vorlesung. Jede Übung baut auf den vorherigen auf und deckt verschiedene Aspekte des Deep Learning ab.

## Übungsstruktur

### 📚 Übung 1: Mathematische Grundlagen und Einführung
- **Themen**: Lineare Algebra, Aktivierungsfunktionen, Perceptron, XOR-Problem
- **Schwerpunkt**: Mathematische Fundamente, erste Implementierungen
- **Bearbeitungszeit**: 2 Wochen
- **Punkte**: 85 + 10 Bonus

**Lernziele:**
- Verstehen der mathematischen Grundlagen
- Implementierung von Aktivierungsfunktionen
- Lösung des XOR-Problems mit MLPs
- Grundlagen der Gradientenberechnung

### 🧠 Übung 2: Multi-Layer Perceptrons und Backpropagation
- **Themen**: Backpropagation-Algorithmus, MLP-Implementierung, Vanishing Gradients
- **Schwerpunkt**: Tieferes Verständnis des Lernprozesses
- **Bearbeitungszeit**: 3 Wochen
- **Punkte**: 85 + 15 Bonus

**Lernziele:**
- Mathematische Herleitung von Backpropagation
- Vollständige MLP-Implementierung von Grund auf
- Experimentelle Evaluierung verschiedener Architekturen
- Verstehen von Overfitting und Regularisierung

### 🖼️ Übung 3: Convolutional Neural Networks (CNNs)
- **Themen**: 2D-Convolution, Pooling, CNN-Architekturen, Computer Vision
- **Schwerpunkt**: Bildverarbeitung und räumliche Strukturen
- **Bearbeitungszeit**: 3 Wochen
- **Punkte**: 105 + 15 Bonus

**Lernziele:**
- Mathematik der Convolution-Operation
- CNN-Implementierung für Bildklassifikation
- Verstehen von Feature Maps und hierarchischem Lernen
- Praktische Anwendung auf MNIST

### 🔄 Übung 4: Recurrent Neural Networks und Sequence Modeling
- **Themen**: RNNs, LSTMs, BPTT, Attention, Sequence-to-Sequence
- **Schwerpunkt**: Zeitreihendaten und sequentielle Modellierung
- **Bearbeitungszeit**: 3 Wochen
- **Punkte**: 105 + 15 Bonus

**Lernziele:**
- Backpropagation Through Time (BPTT)
- LSTM-Architektur und Gating-Mechanismen
- Anwendungen auf Zeitreihen und Textgeneration
- Attention-Mechanismen

### 🎨 Übung 5: Generative Modelle und Advanced Deep Learning
- **Themen**: Autoencoders, VAEs, GANs, Transfer Learning
- **Schwerpunkt**: Generative Modellierung und praktische Anwendungen
- **Bearbeitungszeit**: 4 Wochen
- **Punkte**: 105 + 45 Bonus/Projekt

**Lernziele:**
- Variational Autoencoders und probabilistische Modellierung
- Generative Adversarial Networks und Spieltheorie
- Praktische Deep Learning Techniken
- End-to-End Projektarbeit

## 📋 Voraussetzungen

### Mathematische Grundlagen
- **Lineare Algebra**: Matrixoperationen, Eigenwerte, Normen
- **Analysis**: Partielle Ableitungen, Kettenregel, Optimierung
- **Statistik**: Wahrscheinlichkeitstheorie, Verteilungen
- **Numerik**: Numerische Stabilität, Finite Differenzen

### Programmierkenntnisse
- **Python**: Grundlagen, OOP, NumPy, Matplotlib
- **Datenstrukturen**: Arrays, Listen, Dictionaries
- **Algorithmen**: Gradient Descent, Backpropagation
- **Optional**: PyTorch/TensorFlow für erweiterte Aufgaben

## 🛠️ Technische Umgebung

### Erforderliche Bibliotheken
```python
# Kern-Bibliotheken
import numpy as np
import matplotlib.pyplot as plt
import scipy.stats

# Datenverarbeitung
from sklearn.datasets import fetch_openml, make_classification
from sklearn.model_selection import train_test_split
from sklearn.metrics import classification_report

# Erweiterte Visualisierung
import seaborn as sns

# Optional für Bonusaufgaben
import torch
import tensorflow as tf
```

### Installation
```bash
pip install numpy matplotlib scipy scikit-learn seaborn
# Optional:
pip install torch torchvision tensorflow
```

## 📊 Bewertungssystem

### Punkteverteilung
| Übung | Grundpunkte | Bonuspunkte | Gesamt |
|-------|-------------|-------------|---------|
| 1 | 85 | 10 | 95 |
| 2 | 85 | 15 | 100 |
| 3 | 105 | 15 | 120 |
| 4 | 105 | 15 | 120 |
| 5 | 105 | 45 | 150 |
| **Gesamt** | **485** | **100** | **585** |

### Notenschlüssel
- **1,0-1,3 (Sehr gut)**: 90-100% der Grundpunkte
- **1,7-2,3 (Gut)**: 75-89% der Grundpunkte
- **2,7-3,3 (Befriedigend)**: 60-74% der Grundpunkte
- **3,7-4,0 (Ausreichend)**: 50-59% der Grundpunkte

### Bonuspunkte
- Bonuspunkte können Grundpunkte kompensieren
- Maximale Gesamtnote: 1,0
- Besonders kreative Lösungen werden extra gewürdigt

## 📝 Abgaberichtlinien

### Format
- **Code**: Jupyter Notebooks (.ipynb) mit vollständiger Ausführung
- **Mathematik**: PDF-Dokument mit LaTeX-formatierten Herleitungen
- **Diskussion**: Interpretation der Ergebnisse und Beobachtungen
- **Plots**: Alle Visualisierungen mit Beschriftung

### Struktur
```
abgabe_uebungX_nachname/
├── uebungX_nachname.ipynb    # Hauptnotebook
├── mathematik_uebungX.pdf    # Mathematische Herleitungen
├── ergebnisse/               # Generierte Plots und Modelle
│   ├── plots/
│   └── models/
└── README.md                 # Kurze Zusammenfassung
```

### Qualitätskriterien
- **Reproduzierbarkeit**: Code läuft ohne Fehler durch
- **Dokumentation**: Ausführliche Kommentare und Markdown
- **Mathematik**: Vollständige, korrekte Herleitungen
- **Analyse**: Kritische Diskussion der Ergebnisse

## 🎯 Lernstrategie

### Empfohlenes Vorgehen
1. **Theorie zuerst**: Verstehen Sie die mathematischen Grundlagen
2. **Kleine Schritte**: Implementieren Sie zunächst einfache Versionen
3. **Testen**: Verwenden Sie kleine, bekannte Datensätze zum Debugging
4. **Visualisieren**: Plotten Sie Zwischenergebnisse für besseres Verständnis
5. **Experimentieren**: Variieren Sie Hyperparameter systematisch

### Häufige Probleme und Lösungen
- **Numerische Instabilität**: Verwenden Sie numerisch stabile Implementierungen
- **Overfitting**: Implementieren Sie Regularisierung und Cross-Validation
- **Debugging**: Überprüfen Sie Dimensionen und Gradienten numerisch
- **Performance**: Optimieren Sie erst nach korrekter Implementierung

## 🤝 Zusammenarbeit

### Erlaubt
- Diskussion von Konzepten und Ansätzen
- Gemeinsames Debugging von Implementierungsproblemen
- Austausch von Referenzen und Ressourcen
- 2er-Teams für Brainstorming (individuelle Abgabe!)

### Nicht erlaubt
- Kopieren von Code oder mathematischen Herleitungen
- Austausch von kompletten Lösungen
- Verwendung von ChatGPT/KI für direkte Lösungsgenerierung
- Plagiate jeder Art

## 📚 Zusätzliche Ressourcen

### Empfohlene Literatur
- **Deep Learning** - Ian Goodfellow, Yoshua Bengio, Aaron Courville
- **Pattern Recognition and Machine Learning** - Christopher Bishop
- **Neural Networks for Pattern Recognition** - Christopher Bishop

### Online-Ressourcen
- [Deep Learning Specialization - Coursera](https://www.coursera.org/specializations/deep-learning)
- [CS231n - Stanford](http://cs231n.stanford.edu/)
- [Distill.pub](https://distill.pub/) - Interaktive ML-Artikel
- [Papers with Code](https://paperswithcode.com/) - SOTA-Implementierungen

### Implementierungsbeispiele
- [Andrej Karpathy's Blog](http://karpathy.github.io/)
- [Christopher Olah's Blog](http://colah.github.io/)
- [Sebastian Ruder's Blog](https://ruder.io/)

## 🆘 Hilfe und Support

### Sprechstunden
- **Wann**: Dienstags 14:00-16:00
- **Wo**: Büro XYZ oder online
- **Anmeldung**: Per E-Mail im Voraus

### E-Mail Support
- **Antwortzeit**: Innerhalb von 24-48 Stunden
- **Format**: Spezifische Fragen mit Code-Snippets
- **Betreff**: "DL Übung X - Kurze Beschreibung"

### Peer Learning
- **Discord/Slack**: Gemeinsamer Kanal für Diskussionen
- **Study Groups**: Selbstorganisierte Lerngruppen
- **Office Hours**: Offene Fragestunden vor Abgabeterminen

## 🏆 Erfolg messen

### Nach jeder Übung sollten Sie können:
- **Übung 1**: Grundlegende neuronale Netze von Grund auf implementieren
- **Übung 2**: Komplexe Architekturen entwerfen und trainieren
- **Übung 3**: Computer Vision Probleme mit CNNs lösen
- **Übung 4**: Sequentielle Daten mit RNNs/LSTMs modellieren
- **Übung 5**: Generative Modelle verstehen und anwenden

### Portfolio-Entwicklung
Am Ende des Kurses haben Sie:
- Ein vollständiges Deep Learning Framework implementiert
- Mehrere praktische Anwendungen entwickelt
- Tiefes Verständnis der mathematischen Grundlagen
- Fähigkeit zur kritischen Analyse von ML-Modellen
- Basis für fortgeschrittene Deep Learning Forschung

---

**Viel Erfolg bei den Übungen! 🚀**

Bei Fragen stehen wir gerne zur Verfügung.