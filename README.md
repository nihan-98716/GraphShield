# GraphShield 🛡️
### AI-Powered Enterprise Cyber Contagion Simulator

GraphShield models ransomware propagation across enterprise network 
graphs, detects anomalous behavior using Isolation Forest, compares 
adaptive defense strategies, and generates LLM-powered threat 
intelligence reports.

---

## Architecture
```
Graph Engine → Propagation → Anomaly Detection → Risk Analysis
                                    ↓
                    Defense Simulator → Report Generator
```

## Modules
| File | Purpose |
|---|---|
| network_graph.py | BA scale-free network generation |
| propagation_engine.py | SIR malware spread simulation |
| anomaly_detector.py | IsolationForest behavioral detection |
| risk_engine.py | Centrality-based risk scoring |
| defense_simulator.py | 6-strategy defense comparison |
| report_generator.py | LLM threat assessment reports |
| ai_modules.py | GNN + RL architectural stubs |
| main.py | Full pipeline orchestrator |

## Installation
```bash
git clone https://github.com/yourusername/graphshield
cd graphshield
pip install -r requirements.txt
```

## Configuration
Create a `.env` file:
```
GEMINI_API_KEY=your_key_here
# or
OLLAMA_MODEL=llama3.2
```

## Usage
```bash
# Run full pipeline
python main.py --scenario all --attacker greedy --visualize

# Single scenario
python main.py --scenario finance --attacker greedy

# Skip LLM report
python main.py --scenario all --no_report
```

## Attack Scenarios
| Scenario | Entry Point | Attacker |
|---|---|---|
| random | Random workstation | Random |
| finance | Finance dept server | Greedy |
| dc | Domain controller | Greedy |
| stealth | Random node | Stealth |

## Defense Strategies Compared
- No Defense (baseline)
- Random Patching
- Vulnerability-Based Patching
- Centrality-Based Patching
- Bridge Node Isolation
- Anomaly-Guided Patching (AI)

## AI Components
- **Isolation Forest** — unsupervised behavioral anomaly detection
- **LLM Report Generation** — Gemini/Ollama threat assessment
- **GNN stub** — GraphSAGE infection prediction (future)
- **RL stub** — PPO adaptive defense agent (future)

## Output
- Network infection spread visualization
- Risk heatmap
- Defense strategy comparison charts
- Detection timeline plots
- LLM-generated threat assessment reports

## Future Work
- GNN-based infection path prediction
- Reinforcement Learning defense optimization
- Real network topology integration

## License
MIT License — see LICENSE file
