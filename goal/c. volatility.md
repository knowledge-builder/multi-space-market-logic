### 2. Volatility Proxies

**What they are:**
Not “volatility” in finance terms.

**They are:**
measurements of movement intensity in the derivative space

**Examples:**
* step_move
* scale (rolling abs returns)
* range measures

**Function in your system:**
They define:
* the energy level of the system

Not direction — just intensity.

**Why they matter:**
They answer:
* “How much is the system changing right now?”

**Without them:**
* you cannot distinguish calm structure vs chaotic structure
* distance alone becomes meaningless

**With them:**
* you normalize all state deviations by movement capacity

This is why your reversion = distance / scale works.
