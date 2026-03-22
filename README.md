# Opencode 100+ Advanced Agents Pack

[![GitHub stars](https://img.shields.io/github/stars/MukeshMakvana1/opencode-agents-pack?style=social)](https://github.com/MukeshMakvana1/opencode-agents-pack)

## 🎯 Introduction

This repository provides **100+ advanced AI agents** for [Opencode](https://opencode.ai) - a powerful agentic coding terminal. Each agent specializes in specific domains with **detailed skills, workflows, code examples, and best practices**.

### Key Features
- **25+ categories** (expandable to 105)
- **500+ specialized skills**
- **Ready-to-use** .md agent files
- **Valid model configs** (`opencode/minimax-m2.5-free`)
- **Cross-platform** Windows/macOS/Linux

**Agents cover:** DevOps (Kubernetes, Docker), Security (Pentesting, Crypto), Data Science (Pandas, Spark), Blockchain (Solidity, DeFi), Game Dev (Unity, Unreal), and more!

## 📦 Installation

### Prerequisites
- [Opencode](https://opencode.ai) installed
- Windows 10/11

### One-Click Install (Recommended)
Download `agents-pack.zip` from [releases](https://github.com/MukeshMakvana1/opencode-agents-pack/releases)
2. Extract to `%USERPROFILE%\.opencode\agents` (creates subfolders)
3. Run `opencode` - agents auto-load!

```
C:\Users\YourName\.opencode\agents\
├── devops\
│   ├── kubernetes-expert.md
│   └── ...
├── security\
└── ...
```

### Manual Install
1. Clone repo:
   ```
   git clone https://github.com/badgeshaas/opencode-agents-pack.git
   ```
2. Copy `agents/` to `~/.opencode/agents/` (Linux/macOS) or `%USERPROFILE%\.opencode\agents\` (Windows)
3. Restart Opencode

## 🚀 Usage

### Switching Agents
```
# Prefix with @
@python-developer write a Flask API
@kubernetes-expert deploy nginx on EKS
@penetration-tester scan for XSS vulns

# Cycle agents
agent.cycle

# List agents
agent
```

### Example Sessions
**DevOps Kubernetes Deployment:**
```
@devops-kubernetes-expert
Create a production nginx deployment with HPA, Ingress, and monitoring
```

**Security Audit:**
```
@security-penetration-tester
Burp Suite workflow for OWASP Top 10 testing on example.com
```

**Data Analysis:**
```
@data-science-pandas-pro
Load sales.csv, compute YoY growth, plot dashboard
```

## 🗂️ Agent Categories (25+ Agents)

| Category | Agents | Skills |
|----------|--------|--------|
| DevOps | 5 | Kubernetes, Docker, CI/CD, AWS, Terraform |
| Security | 5 | Pentesting, SIEM, Crypto, Firewall, IR |
| Data Science | 5 | Pandas, Spark, Tableau, ETL, Features |
| Blockchain | 5 | Solidity, Web3, Audits, DeFi, NFTs |
| Game Dev | 5 | Unity, Unreal, Godot, AI, Netcode |
| ... (20 more) | 85+ | Full list in TODO.md |

### Full Agent List
See [TODO.md](TODO.md) for progress and details.

## ⚙️ Configuration

Agents use standard format:
```yaml
---
name: agent-name
description: Short desc
mode: all
model: opencode/minimax-m2.5-free
temperature: 0.6
tools:
  write: true
  bash: true
---
Detailed skills...
```

### Custom Models
Edit model line:
```
model: opencode/gpt-5-nano  # Faster
model: opencode/big-pickle  # Powerful
```

Run `opencode models` for list.

## 🛠️ Troubleshooting

**Model Invalid?**
- Run `opencode models` - use exact ID
- Restart Opencode after changes

**Agents Not Loading?**
```
ls ~/.opencode/agents -R
opencode --log-level DEBUG
```

**Windows Path Issues?**
```
dir %USERPROFILE%\.opencode\agents
```

**YAML Errors?**
- Validate with YAML lint
- Check indentation (2 spaces)

## 🔧 Development

Add new agents:
1. Create `category/agent-name.md`
2. Follow template above
3. Test with `opencode`

Contribute: [Pull Requests Welcome](https://github.com/badgeshaas/opencode-agents-pack/pulls)

## 📄 License
MIT License - see [LICENSE](LICENSE)

## 🙌 Acknowledgments
- [Opencode AI](https://opencode.ai)
- Community contributors

---

⭐ **Star on GitHub** | 🔔 **Watch releases** | 💬 **Issues/Discussions**

**Made with ❤️ for AI developers worldwide**

