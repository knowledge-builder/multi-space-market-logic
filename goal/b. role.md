## 2. The real role of each component

### 🟦 1. Rolling Statistics
**What they are in a system sense:**
Local “views” of the system’s state over a moving window.

**They define:**
- short-term equilibrium (mean)
- short-term variability (scale)
- short-term structure (distribution shape)

**Function in your system:**
They act as:
- a local coordinate system generator

**Every window creates a temporary “world” where:**
- what is normal
- what is extreme
- what is balanced
is redefined

**Why they matter:**
- **Without rolling stats:**
    - the system has no notion of “local reality”
    - everything becomes globally averaged (which destroys structure)
- **With rolling stats:**
    - you get evolving frames of reference
