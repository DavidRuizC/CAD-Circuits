
# 🔌 Logic Circuit Simulator in Python

This project is a **step-by-step evolution** of a Python-based digital logic circuit simulator. It showcases how abstract design patterns and object-oriented principles can be used to simulate logic gates and components such as XOR, AND, OR, NOT, and full multi-bit adders.

## 🚀 Overview

The simulator progresses from simple logic gates to complex components including:
- XOR gates
- 1-bit, 4-bit, and 8-bit adders
- Observable and reactive pin connections using the Observer pattern

Each `stepX.py` file introduces enhancements and new concepts, building upon the previous version.

## 📁 Project Structure

- `step1.py` → Basic AND gate with input/output handling
- `step2.py` → Introduction of Circuit class and basic logic gates as components
- `step3.py` → Use of Pin abstraction and I/O structure
- `step4.py` → Observer pattern for reactive pin behavior (Pin = Observable + Observer)
- `step5.py` → Implemented logic for AND, OR, NOT, and component `process` methods
- `step6.py` → Functional testing of AND gate and XOR component
- `step7.py` → Construction of:
  - ✅ 1-bit adder using multiple logic gates
  - ✅ 4-bit adder using 1-bit adder modules
  - ✅ 8-bit adder using 4-bit adder modules

## 🧠 Concepts Used

- **Composite Pattern**: For creating hierarchical circuit structures
- **Observer Pattern**: For real-time signal propagation between pins
- **Encapsulation and Modularity**: Each circuit and pin manages its own logic and connections
- **Deep Copy**: Used to replicate and reuse adder components at different scales

## ▶️ How to Run

To execute a particular step:

```bash
python stepX.py
# Replace X with 1–7, depending on the version you want to test
```

The final version `step7.py` demonstrates a fully working **8-bit adder**.

## 🧪 Example Output

```plaintext
ONE BIT ADDER
True + True + False = False, True

FOUR BIT ADDER
7 + 8 + 1 = 16, True

EIGHT BIT ADDER
255 + 1 + 0 = 256, True
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
