# 🕵️ Perry the Platypus Perplexity Calculator

> **Live Demo:** [https://perry-perplexity-calculator.vercel.app](https://perry-perplexity-calculator.vercel.app)

An interactive, light-themed **Perplexity Calculator** built with modern **Glassmorphism**, featuring **Perry the Platypus (Agent P)** from *Phineas and Ferb*!

---

## ✨ Features

- 🧮 **Formal Perplexity Calculation**: Calculates perplexity using the natural language processing equation:
  $$\text{PPL}(W) = P(w_1, w_2, \dots, w_N)^{-\frac{1}{N}} = \exp\left( -\frac{1}{N} \sum_{i=1}^N \ln P(w_i) \right)$$
- 🔍 **Interactive Word Probabilities**:
  - Live tokenization for any input sentence.
  - Automatically assigns independent random probabilities to each word.
  - Fine-tune probabilities manually using numeric inputs or visual range sliders.
  - Quick-preset buttons (`High 0.9`, `Med 0.5`, `Low 0.1`, `Rare 0.02`).
- 🦆 **Perry the Platypus (Agent P) Emotes**:
  - Custom vector SVG illustration of Agent P wearing his iconic brown fedora.
  - **Dynamic Thinking Cloud**: The thinking cloud (`🤔 Thinking...`) pops up strictly while you are adjusting probabilities.
  - **Idle Greeting**: Reverts to *"Hello, I'm Perry the Platypus"* when idle.
- 💎 **Modern Glassmorphism Design**: Frosted glass cards (`backdrop-filter: blur(16px)`), pastel teal/cream/orange palette, and ambient gradient glows.
- 📊 **Step-by-Step Breakdown Table**: Inspect token index, word $w_i$, probability $P(w_i)$, surprisal in nats ($-\ln P(w_i)$), and information in bits ($-\log_2 P(w_i)$).

---

## 🚀 Live Deployment

The application is deployed on Vercel:
**[https://perry-perplexity-calculator.vercel.app](https://perry-perplexity-calculator.vercel.app)**

---

## 🛠️ Local Development

Simply clone the repository and open `index.html` in your browser:

```bash
git clone https://github.com/littlecinnabun/perry-perplexity-calculator.git
cd perry-perplexity-calculator
open index.html
```

Or run a local static server:
```bash
python3 -m http.server 8080
```
Then visit `http://localhost:8080`.
