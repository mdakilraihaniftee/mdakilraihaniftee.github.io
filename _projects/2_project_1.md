---
layout: page
title: Ludo 2.0
description: Python-Based Human vs AI Board Game
img: assets/img/ludo.png
importance: 2
category: Development Projects
related_publications: false
giscus_comments: true
---

# Ludo 2.0

**Ludo 2.0** is a Python-based AI-powered board game, simulating a one-on-one match between a human player and an intelligent AI. The AI learns and predicts optimal moves by analyzing human gameplay behavior using **Decision Tree Classifier** and applying **Fuzzy Logic** for uncertain or strategic game decisions.

<div class="col-sm mt-3 mt-md-0">
  {% include figure.liquid path="assets/img/ludo_t.png" title="Ludo 2.0 AI Gameplay" class="img-fluid rounded z-depth-1" %}
</div>

## Key Features

- 🎲 Human vs AI Ludo gameplay
- 🧠 AI decision-making using machine learning and fuzzy logic
- 📊 Prediction of optimal moves based on historical strategies
- 🔄 Turn-based movement with intelligent prioritization
- 📁 Modular code to extend multi-player or multi-agent logic

---

## Project Showcase

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ludo_board.png" title="Ludo Board Engine" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ludo_brain.png" title="AI Brain Logic" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  Left: In-game Ludo board simulation | Right: AI Move Prediction via Decision Tree + Fuzzy Logic
</div>

---

## Live Demo & Source

- 💻 GitHub Repository: [Ludo 2.0 on GitHub](https://github.com/mdakilraihaniftee/Ludo-2.0)
- 🎥 Gameplay: Command-line based interaction
- 🚧 _Note_: GUI and multiplayer extensions are under consideration for future versions.

---

## Tech Stack

- **Language**: Python 3  
- **ML Model**: Scikit-learn (Decision Tree Classifier)  
- **Fuzzy Logic**: Custom rule-based reasoning  
- **Execution**: CLI-based interaction  
- **Data Handling**: NumPy arrays for move and state logic  

---

<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ludo_ai_move.png" title="AI Optimal Move Decision" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/ludo_tree.png" title="Decision Tree Snapshot" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

<div class="caption">
  Visualization of AI choosing optimal token movement based on fuzzy scores and decision path
</div>

---

> _This project demonstrates how AI can be combined with traditional board games to create intelligent, adaptive opponents. Built for fun, challenge, and machine learning experimentation._
