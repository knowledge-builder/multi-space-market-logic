## 1. First principle (we anchor everything here)

A feature is never meaningful by itself.
It is only meaningful inside a defined space.

So before we touch anything else, we lock this rule:

A system is defined by:
* what counts as a state
* what counts as a change
* what counts as a history (memory)

Everything else is derived.

## 2. Your system already has 3 spaces (we formalize them properly)

### STATE SPACE (geometry of the system)
This is the “where is price?”

**Objects:**
* close (current state)
* mean (local equilibrium)
* median (robust center)

**Derived:**
* distance = |close − mean|
* distortion = |mean − median|

**Meaning:**
This space answers: “Where is the system relative to its internal reference points?”

### DERIVATIVE SPACE (movement of the system)
This is “how is the system moving?”

**Objects:**
* step_move = |Δclose|
* scale = rolling mean(step_move)

**Meaning:**
This space does NOT describe price. It describes how fast state is changing.

**Important:**
* scale is NOT volatility as a label
* it is a local unit of motion

### BEHAVIOR SPACE (time distribution of state)
This is “how does the system behave over time?”

**Objects:**
* n_above_mean
* n_below_mean
* imbalance

**Meaning:**
This space ignores magnitude and focuses on time occupancy patterns.

## 3. Now the key correction (this is where everything becomes clear)

You previously tried:
scale ↔ distance relationship

That is invalid because:
* distance belongs to STATE space
* scale belongs to DERIVATIVE space

So they are:
not comparable quantities — they are different coordinate systems.

## 4. What actually connects spaces (very important)

Spaces are connected only through:
**Cross-space mappings (NOT direct comparisons)**

You already created two:

1.  **Reversion (STATE → DERIVATIVE mapping)**
    * reversion = distance / scale
    * **Meaning:** “How large is this position relative to current movement capacity?”
    * This is not a feature — it is a unit conversion across spaces.

2.  **Structural compression (STATE structure → DERIVATIVE normalization)**
    * C = distortion / scale
    * **Meaning:** “How significant is structural imbalance relative to movement intensity?”

## 5. The mental shift you must lock in

Stop thinking:
“What is the relationship between features?”

Start thinking:
“What space generated this feature, and what transformation makes it comparable to another space?”

## 6. A simple rule to prevent future confusion

Before comparing anything, ask:

* **Step 1:** What space does each variable belong to?
* **Step 2:** Are they in the same space?
    * yes → direct comparison allowed
    * no → must define transformation
* **Step 3:** What transformation makes them comparable?
    * normalization
    * ratio
    * z-score
    * scaling by local unit (your scale variable)

## 7. Your system in one clean equation form

You are building this:
* STATE space → (structure)
* DERIVATIVE space → (movement)
* BEHAVIOR space → (time distribution)

**Cross-space operators:**
* STATE ÷ DERIVATIVE → significance
* STATE structure ÷ DERIVATIVE → stability

## 8. Now your next step (important)

Now that the structure is clean, the next logical question is:
what is the minimum set of independent spaces needed so your system is complete without redundancy?

Because right now:
some of your variables may be redundant projections of the same structure.
