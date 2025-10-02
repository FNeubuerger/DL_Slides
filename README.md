# Neural Networks & Deep Learning - Vorlesungsfolien

[![LaTeX](https://img.shields.io/badge/LaTeX-beamer-blue.svg)](https://github.com/FNeubuerger/DL_Slides)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📚 Über diese Vorlesung

Diese Vorlesung bietet eine umfassende Einführung in **Neural Networks** und **Deep Learning**. Die Folien kombinieren theoretische Grundlagen mit praktischen Anwendungen und enthalten ausführliche mathematische Herleitungen.

## 🎯 Lernziele

Nach dieser Vorlesung können Studierende:
- Mathematische Grundlagen neuronaler Netze verstehen und anwenden
- Verschiedene Netzarchitekturen (MLP, CNN, RNN, LSTM, VAE, GAN) erklären
- Backpropagation-Algorithmus mathematisch herleiten
- Praktische Entscheidungen zwischen Deep Learning und klassischem ML treffen

## 📖 Inhalt der Vorlesung

### 1. Mathematische Grundlagen (Folien 1-50)
- **Lineare Algebra Refresher**: Vektoren, Matrizen, Eigenwerte
- **Analysis**: Gradienten, partielle Ableitungen, Kettenregel
- **Wahrscheinlichkeitstheorie**: Verteilungen, Bayes'sche Statistik
- **Optimierung**: Gradientenabstieg, Konvexität
- **Informationstheorie**: Entropie, KL-Divergenz
- **Statistik**: Hypothesentests, Maximum Likelihood

### 2. Grundlagen Neuronaler Netze (Folien 51-100)
- **Perceptron**: Lineare Klassifikation, mathematische Herleitung
- **Multi-Layer Perceptron (MLP)**: Universal Approximation Theorem
- **Aktivierungsfunktionen**: Sigmoid, ReLU, Softmax
- **Backpropagation**: Mathematische Herleitung und Implementierung
- **Verlustfunktionen**: Cross-Entropy, Mean Squared Error

### 3. Deep Learning Architekturen (Folien 101-200)
- **Convolutional Neural Networks (CNNs)**:
  - Convolution Operation und mathematische Grundlagen
  - Pooling, Feature Maps, Translation Equivarianz
  - Anwendungen in Computer Vision
- **Recurrent Neural Networks (RNNs)**:
  - Sequentielle Datenverarbeitung
  - Vanishing Gradient Problem
- **Long Short-Term Memory (LSTM)**:
  - Gate-Mechanismen, Cell State
  - Mathematische Herleitung der Forget-, Input- und Output-Gates

### 4. Generative Modelle (Folien 201-250)
- **Variational Autoencoders (VAEs)**:
  - Evidence Lower Bound (ELBO)
  - Reparameterization Trick
  - Latente Repräsentationen
- **Generative Adversarial Networks (GANs)**:
  - Adversarial Training, Minimax-Spiel
  - Lipschitz-Constraint und WGAN
  - Mode Collapse und Lösungsansätze

### 5. Praktische Anwendungen (Folien 251-300)
- **Wann Deep Learning vs. klassisches ML?**: Praktische Entscheidungshilfen
- **Projektarbeit**: Hands-on Erfahrung mit realen Datensätzen

## 🛠️ Technische Details

- **LaTeX Engine**: LuaLaTeX (empfohlen für Unicode-Unterstützung)
- **Document Class**: Beamer für Präsentationen
- **Sprache**: Deutsch (mit Polyglossia)
- **Mathematik**: umfangreiche Nutzung von amsmath, mathtools
- **Bibliographie**: BibTeX mit DOI-Links für alle Referenzen

## 🚀 Kompilierung

### Voraussetzungen
- TeX Live 2024 oder später
- LuaLaTeX Engine
- Folgende LaTeX-Pakete: `beamer`, `polyglossia`, `amsmath`, `mathtools`, `csquotes`, `smartdiagram`

### Kompilieren
```bash
# Mit latexmk (empfohlen)
latexmk -lualatex -synctex=1 -interaction=nonstopmode main.tex

# Manuell
lualatex main.tex
bibtex main
lualatex main.tex
lualatex main.tex
```

## 📁 Projektstruktur

```
DL_Slides/
├── main.tex                 # Hauptdokument
├── lit.bib                  # Bibliographie mit DOIs
├── beamerthemefhswf.sty     # Hochschul-Theme
├── images/                  # Alle Abbildungen und Diagramme
│   ├── CNN.png
│   ├── LSTM_*.png
│   ├── GAN.png
│   └── ...
├── logos/                   # Hochschul-Logos
└── README.md               # Diese Datei
```

## 🎓 Für Studierende

### Empfohlene Vorbereitung
- Grundlagen in Python und NumPy
- Lineare Algebra und Analysis (Refresher in der Vorlesung enthalten)
- Interesse an mathematischen Herleitungen

## 📚 Weiterführende Ressourcen

- **Bücher**:
  - Goodfellow, I., Bengio, Y., Courville, A.: "Deep Learning" (MIT Press)
  - Bishop, C.: "Pattern Recognition and Machine Learning"
- **Online-Kurse**:
  - CS231n: Convolutional Neural Networks (Stanford)
  - CS224n: Natural Language Processing (Stanford)
- **Praktische Tools**:
  - PyTorch, TensorFlow
  - Jupyter Notebooks
  - Google Colab für GPU-Zugang

## 🤝 Contributing

Verbesserungsvorschläge und Fehlerkorrekturen sind willkommen:
1. Fork das Repository
2. Erstelle einen Feature-Branch (`git checkout -b feature/improvement`)
3. Committe deine Änderungen (`git commit -am 'Add improvement'`)
4. Push zum Branch (`git push origin feature/improvement`)
5. Erstelle einen Pull Request

## 📄 Lizenz

Dieses Projekt steht unter der MIT-Lizenz - siehe [LICENSE](LICENSE) für Details.

## 👨‍🏫 Autor

**Felix Neubürger**  
Fachhochschule Südwestfalen  
Fachbereich Informatik und Naturwissenschaften

---

*Diese Vorlesung wurde entwickelt, um Studierenden eine solide theoretische Grundlage und praktische Erfahrung im Bereich Deep Learning zu vermitteln.*