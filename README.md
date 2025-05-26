[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/madara88645/entangled-ai-3.0/blob/main/en3.ipynb)



# Entangled Learning 3.0 — CNN Teacher with Dual MLP Students via JS Divergence

This project demonstrates a novel **entangled learning setup** where:
- A **CNN teacher** model is trained on full-resolution CIFAR-10 images.
- Two **small MLP students** learn from **PCA-compressed inputs**.
- All models are aligned through **Jensen-Shannon divergence** between their predictions.
- Alignment strength **λ increases over epochs**, and eventually transitions from soft (JS) to hard (label) imitation.

> 🎯 **Goal:** Improve low-capacity models by aligning with a high-capacity teacher — without sharing raw data or layers.

---

## 🔬 Highlights

- 📦 Dataset: CIFAR-10  
- 🧠 Models:
  - CNN (Teacher)
  - MLP Small B (64 units, PCA input)
  - MLP Small C (32 units, alternate PCA input)
- 🔁 Learning Signals:
  - Cross-Entropy (True Labels)
  - Jensen-Shannon Divergence (Teacher ↔ Students)
  - Student-Student Mutual Entanglement (optional)
- 📈 Metrics: Loss, Accuracy, ROC-AUC (macro)
- 📉 λ (JS Weight): Increases logarithmically during training

---

## 📊 Visualization

4-panel plot shows:
- Training loss
- Test accuracy
- Test ROC-AUC
- Entanglement λ progression

---

📎 Example Use-Cases
Collaborative learning with edge models

Distillation without logits transfer

Hybrid teacher-student systems

Multi-agent learning

📄 Reference
Mehmet Özel. Entangled Learning 3.0: Teaching Tiny Models to Think Better with Jensen-Shannon Guidance, 2024
📖 Read the full article on: 
[Medium](https://medium.com/@mehmet.ozel2701/entangled-learning-3-0-collaborative-neural-networks-without-sharing-weights-33b45f3cfc34)


📧 Contact
For questions or collaborations, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/mehmet-özel-695227300/)



