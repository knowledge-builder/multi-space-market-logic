## 2. CHANGE = “what transforms state into another state”

Change is:
- the rule that connects one state to the next

In your system:
- step_move = close[t] − close[t−1]
- scale = rolling average of step_move

### Intuition to develop:
- Think: “What is the mechanism that moves the system forward in time?”

### Key insight:
- Change is not data — it is a transition rule

Without it:
- you only have disconnected snapshots
- no dynamics
- no system
