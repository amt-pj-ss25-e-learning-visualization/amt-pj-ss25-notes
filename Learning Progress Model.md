# Learning Progress Model

## 1. Completion Rate

```(Completed Submodules / Total Submodules in the Course) * 100```

**Notes:**

Represents how much of the course content a learner has completed in percentage.

---

## 2. Mastery Level

```Evaluated Verb Score * Difficulty```

**Notes:**

Indicates how well the learner is doing in a module based on self-reflection while considering the module difficulty. This rating can be done not only after completing a module, but also in the meantime.

- **Evaluated Verb Score:** The result associated with the verb *"Evaluated"* in xAPI-Statements: How the learner self-reflected his current progress/understanding for a specific module.
- **Difficulty:** Aggregated difficulty rating (mapped from the existing difficulty-value in LOM to numeric values) of all learning resources linked to the specific module.

---

## 3. Performance Level

```Achieved Score * Difficulty```

**Notes:**

Indicates how well the learner performed based on actual results after a module completion, considering both their achieved score and the difficulty. Again, the difficulty is aggregated 

---

## Overall Learning Progress

(Weight₁ * Completion Rate) + (Weight₂ * Mastery Level) + (Weight₃ * Performance Level)

**Notes:**

The specific weights are yet to be determined.

---

## Not Part of Learning Progress (Optionally Displayed in the Dashboard)

### Time on Task

```Aggregated Time Spent / Expected Time```

**Notes:**

- Measures how much time the learner spent on a task compared to the expected duration.
- Expected time is derived from metadata such as `TypicalLearningTime` in LOM.
- Actual time is aggregated via corresponding xAPI-Statements.

---