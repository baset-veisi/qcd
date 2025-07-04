# Quantum Circuits and Devices (QCD)

> **Hands‑on laboratories, projects & exercises in quantum computing with Qiskit**\
>

---

---

## 📂 Repository structure

```
qcd/
├── qiskit/                # Jupyter‑Lab coursework
│   ├── module1/           # Single‑qubit gates & basic algorithms
│   ├── module2/           # Multi‑qubit gates & hardware calibration
│   └── module3/           # Noise models & system characterisation
└── exercises/             # PDF + LaTeX problem sets with full derivations
```

| Path               | What you’ll find              | Skills demonstrated                                                                                    |
| ------------------ | ----------------------------- | ------------------------------------------------------------------------------------------------------ |
| `qiskit/module1/*` | **Lab 1 notebooks** & project | Bloch‑sphere visualisation, single‑qubit unitaries, measurement statistics, Deutsch‑Jozsa mini‑project |
| `qiskit/module2/*` | **Lab 2 notebooks**           | CNOT & CZ gates, transpilation for IBM back‑ends, pulse‑level gate analysis                            |
| `qiskit/module3/*` | **Lab 3 notebooks**           | Noise channels, T1/T2 estimation, randomized benchmarking, error‑mitigation tricks                     |
| `exercises/*`      | TeX sources + PDFs            | Dirac notation drills, tensor‑product algebra, circuit identities, variational‑ansatz proofs           |

---

## ⚡ Quick start

1. **Clone the repo**
   ```bash
   git clone https://github.com/BasetV/QCD.git
   cd QCD
   ```
2. **Create & activate an environment** (optional but recommended)
   ```bash
   python -m venv .venv && source .venv/bin/activate
   ```
3. **Install requirements**
   ```bash
   pip install -r requirements.txt   # or manually: pip install qiskit matplotlib jupyterlab
   ```
4. **Launch JupyterLab**
   ```bash
   jupyter lab
   ```
5. **Open any notebook** under `qiskit/module*/` and run the cells.\
   Most notebooks auto‑detect whether you’re on **IBM Quantum Lab** or a local simulator.

> **Tip:** If you have an IBM Quantum account, add your token to an environment variable `QISKIT_IBM_TOKEN` before running hardware jobs.

---

## 🧩 Highlight notebook — “Quantum System Characterization”

- **Goal:** Extract T1 and T2 for a real qubit, build a simple decoherence model, then apply **readout‑error mitigation** to improve fidelity of a 3‑qubit GHZ state.
- **Outcome:** Achieved \~3× reduction in measured error rate on `ibmq_belem`.
- **Tech used:** `qiskit.pulse`, `qiskit_experiments`, Matplotlib.

> See `qiskit/module3/Laboratory 3 - Quantum system characterization.ipynb`.


> *“In theory there is no difference between theory and practice. In practice, there is.”* — Yogi Berra

