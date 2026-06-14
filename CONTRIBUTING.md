# Contributing to RailMind AI

Thank you for contributing to RailMind AI! This guide will help you get started.

## 🚀 Getting Started

```bash
git clone https://github.com/railmind-ai/railmind.git
cd railmind
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt && pip install -e .
```

## 🌿 Branch Strategy

| Branch | Purpose |
|--------|---------|
| `main` | Stable, production-ready code |
| `develop` | Active development |
| `feature/your-feature` | New features |
| `fix/issue-number` | Bug fixes |

## 🧪 Running Tests

```bash
python tests/test_all.py        # Quick run (no pytest needed)
pytest tests/ -v                # With pytest
pytest tests/ -v --cov=src      # With coverage
```

All PRs must pass the full test suite before merging.

## 🎯 Priority Contribution Areas

1. **AI Model Improvements** — Better LSTM/TFT for delay prediction
2. **Real IR Dataset Integration** — IRCTC/CRIS data connectors
3. **Multilingual NLP** — RailGPT support for all 22 scheduled languages
4. **GNN Router** — Graph Neural Network route optimization implementation
5. **Quantum Module** — QAOA timetabling (requires Qiskit)
6. **Simulation Environment** — OpenAI Gym-compatible railway env for RL training
7. **Visualization** — Digital Twin 3D visualization (Three.js / Cesium)

## 📋 Commit Convention

```
feat: add demand surge simulation
fix: DASSE threshold calibration for NFR zone
docs: update digital twin architecture diagram
test: add edge case tests for emergency override
refactor: optimize sensor manager bulk reads
```

## 🔒 Data Privacy

- Never commit real passenger PII data
- Use synthetic/anonymized data in tests and notebooks
- All IRCTC API integrations must comply with India's DPDP Act 2023

## 📄 License

By contributing, you agree your contributions will be licensed under MIT.
