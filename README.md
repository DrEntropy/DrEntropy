

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3000&pause=1000&color=1D9E75&center=true&vCenter=true&repeat=true&width=800&height=60&lines=Ron+%7C+DrEntropy;Semi-retired+tinkerer+with+too+many+interests;Bayesian+everything%2C+ship+sometimes;P(interesting+project+%7C+rabbit+hole)+%E2%89%88+1.0)](https://readme-typing-svg.demolab.com)

---

## 🧠 About Me

Physics Ph.D. building simulation-driven insight tools. Semi-retired, running too many experiments in parallel and updating my priors accordingly. I specialize in Bayesian modeling, ML, and simulation as a tool for understanding and decision-making under uncertainty. Lately thinking about how agentic systems change software development, and where the boundary between simulation and inference really is.

---

## 🎲 Bayesian Self-Portrait

```python
import pymc as pm
import numpy as np

coords = {
    "interest": [
        "Bayesian Modeling", "Machine Learning", "Simulation",
        "RPGs", "Chess", "Learning New Things"
    ],
}

with pm.Model(coords=coords) as ron:
    # Priors
    hours_in_rabbit_hole = pm.Exponential("hours_in_rabbit_hole", lam=0.1)
    time_allocation = pm.Dirichlet("time_allocation", a=[5, 4, 3, 3, 1, 2], dims="interest")

    # What am I working on today?
    current_obsession = pm.Categorical("current_obsession", p=time_allocation)

    # Likelihood — projects per interest
    fun = pm.Deterministic("fun", hours_in_rabbit_hole * time_allocation, dims="interest")
    projects = pm.Poisson("projects", mu=fun, observed=[15, 8, 6, 4, 1, 3], dims="interest")

    idata = pm.sample()  
```

---

## 🚀 Active Projects

**📈 [rationalpursuit.com](https://rationalpursuit.com)** — Data analytics consulting: mathematical modeling, Bayesian methods, and ML

**🤖 Agentic AI** — Claude Code, PydanticAI, OpenRouter — building agents that actually do things
- [`IslandSim`](https://github.com/DrEntropy/IslandSim) — Agentic AI in a tabletop RPG setting — agents making decisions with limited information (WIP)
- [`codecrafters-claude-code-python`](https://github.com/DrEntropy/codecrafters-claude-code-python) — Built my own mini coding agent from the CodeCrafters challenge


**📊 Bayesian & Simulation** — My public repos are just the tip of the iceberg. Topics include PyMC, Stan, diffusion models, reinforcement learning, and agent-based modeling.

**🎲 RPG & Worldbuilding** — Traveller, D&D, Pirate Borg, Dragonbane — player, sometimes GM, always rolling badly

**♟️ Chess** — [admiralentropy on Chess.com](https://chess.com/member/admiralentropy) — long time beginner, playing casually

**📚 Reading** — Perpetual student — Bayesian stats, deep learning, R, causal inference

---

## 🔬 Built to Understand

Things I built because I wanted to know how they actually work.

- [`ParametricEQ`](https://github.com/DrEntropy/ParametricEQ) — Parametric EQ audio plugin in JUCE (C++)
- [`EOPLInterp`](https://github.com/DrEntropy/EOPLInterp) — C++ interpreter from *Essentials of Programming Languages*
- [`ToySOCCore`](https://github.com/DrEntropy/ToySOCCore) — The TOY computer from Sedgewick & Wayne, implemented in VHDL
- [`nexttoken`](https://github.com/DrEntropy/nexttoken) — Interactive next-token prediction visualizer (Hugging Face). "Vibe coded" using Claude.

---

## 🧰 Tools & Toys

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyMC](https://img.shields.io/badge/PyMC-Bayesian-1D9E75?style=for-the-badge)
![Stan](https://img.shields.io/badge/Stan-B2171D?style=for-the-badge)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_Code-Anthropic-D4537E?style=for-the-badge)

---

## 📊 GitHub Stats

![Top Langs by Repo](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=DrEntropy&theme=github_dark)

[![GitHub Streak](https://streak-stats.demolab.com?user=DrEntropy&theme=radical&hide_border=true&background=0D1117&stroke=1D9E75&ring=1D9E75&fire=F8D866&currStreakLabel=1D9E75)](https://streak-stats.demolab.com)

---

## 🌐 Connect

[![rationalpursuit.com](https://img.shields.io/badge/rationalpursuit.com-1D9E75?style=for-the-badge)](https://rationalpursuit.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ronald-legere-a1328796/)

---

<p align="center"><i>"All models are wrong. Some are useful. A few are genuinely fun to build."</i></p>
