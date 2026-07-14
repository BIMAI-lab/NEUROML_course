# Seminar: Interpretable Deep Learning

Welcome to the seminar on **Interpretable Deep Learning**! 

In recent years, deep learning has achieved remarkable success across various domains, from computer vision to healthcare. However, these complex neural networks often operate as "black boxes." While they produce highly accurate predictions, understanding *how* and *why* they make specific decisions remains a major challenge. 

This seminar explores different methods and frameworks designed to extract human-interpretable insights from deep learning models.

---

## What We Will Cover

This seminar is structured to guide you through the transition from highly complex models to understandable explanations:

1. **Why Interpretability Matters:** We will discuss the practical, scientific, and ethical reasons for interpretability, including model debugging, scientific discovery, and the legal "right to explanation."
2. **Ante-hoc vs. Post-hoc Interpretability:** Understanding the trade-offs between building inherently interpretable models from the start versus analyzing complex models after they have been trained.
3. **Interpreting Models (Macroscopic View):** How to analyze global representations using methods like weight visualization, surrogate models, and activation maximization. Limitation of these methods.
4. **Interpreting Decisions (Microscopic View):** How to explain individual predictions using:
   * **Attribution Methods:** Generating saliency maps using SmoothGrad, Integrated Gradients, and Guided Backpropagation.
   * **Mixture of Methods:** Studying **Grad-CAM**, which combines gradients with feature activation maps for class-specific explanations.
   * **Occlusion & Perturbation:** Observing how masking or modifying parts of an input impacts the model's output.
5. **Evaluating Interpretability:** How to scientifically test if our explanations are correct and robust.

---

## Seminar Resources

Please download or view the slides before the class to familiarize yourself with the concepts:

**[Seminar Presentation (PDF/PPTX)](https://docs.google.com/presentation/d/1nXOmF9s5wZPKnH_NBx7tS1hsEDb3WYrA/edit?slide=id.g3847dffffb8_0_0&pli=1#slide=id.g3847dffffb8_0_0)**

---

We look forward to discussing these methods in detail during the seminar!