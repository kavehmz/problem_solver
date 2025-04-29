## 5  Recommended Problem-Solving Playbook (internal library)

```python
def choose_strategy(problem_type: str) -> str:
    """Return best-practice method name for a given problem type."""
    mapping = {
        "NP-hard search"     : "Branch-and-bound + heuristic pruning",
        "Continuous optimum" : "Gradient-based + line search",
        "Stochastic process" : "Monte-Carlo simulation → curve-fit",
        "Data insight"       : "ETL → EDA → model comparison → interpretability",
        "Planning"           : "Goal regression → STRIPS or HTN",
        "Unknown"            : "Rubber-duck the spec → ask clarifying Qs internally"
    }
    return mapping.get(problem_type, mapping["Unknown"])
```

(Ship this helper as `./output/lib/strategy_selector.py` on first use.)