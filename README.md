# AUD&CMA v2 – Ahmet Ulucay Drag-and-Carry Multiplication Algorithm (Version 2)

**AUD&CMA v2** is a generalized digit-wise multiplication algorithm created by **Ahmet Ulucay**, utilizing a **sliding-window convolution method** paired with a unique **drag-and-carry logic**. This version preserves the **leftmost digit** and supports **right-to-left carry propagation**, enabling flexible and efficient multiplication for any integer values.

---

## 🔍 Key Features

- ✅ Supports **any integers** as multiplicands and multipliers
- ✅ Convolution-style **sliding window logic**
- ✅ **Right-to-left carry** with leftmost digit preserved
- ✅ **Binary and decimal system compatibility**
- ✅ Lightweight Python implementation ideal for low-resource environments

---

## 🧠 Concept

In AUD&CMA v2:
- Each digit of the multiplicand is processed using a **sliding window** that overlaps with digits of the multiplier.
- Digits are **zero-padded** symmetrically to align for convolution-style operation.
- Carries propagate **from right to left**, but the **leftmost digit** is **preserved in full**—maintaining readability and traceability.
- Especially useful where digit-wise or bit-wise control is preferred over traditional multiplication.

---

## 💡 Use Cases

- **General-purpose multiplication** for **any integers**, including irregular or mixed-digit patterns
- **Binary and decimal multiplication** where structured digit handling is required
- Simplified **mental arithmetic models** for teaching or manual computation
- **Algorithm visualization** for education or mathematical research
- **Low-power embedded processors** where standard multiplication is costly
- Prototyping **novel arithmetic algorithms** in computer science education or math competitions

---

## 📦 Repository Contents

- `AUDCMA_v2.py` – Python script implementing the core logic of the algorithm
- `examples/` – Sample test cases, expected outputs, and visual diagrams
- `README.md` – Documentation and project overview

---

## 🚀 Quick Start

Clone the repository and run the example code:

```bash
git clone https://github.com/ahmetulucay/AUD-CMA-v2.git
cd AUD-CMA-v2
python AUDCMA_v2.py
