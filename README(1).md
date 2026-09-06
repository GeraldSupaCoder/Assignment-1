# Assignment 1 — Answers

Solutions to Assignment 1, covering four Python questions with explanations and runnable demonstrations for each.

## Contents

The notebook (`Assignment1_Answers.ipynb`) is organized into four sections:

1. **Rate Limiter Bugs (15 marks)** — Debugging a decorator-based rate limiter. Fixes two bugs: a scoping issue where the call-history list was being reassigned instead of mutated in place, and a shared-state issue where all instances of a class incorrectly shared one rate limit instead of each getting its own.

2. **Event Dispatcher / Observer Pattern** — Implementing an `EventDispatcher` class with `subscribe`, `unsubscribe`, and `dispatch` methods. Callbacks run in registration order, and an exception raised by one callback doesn't stop the rest from running.

3. **`Typed` Data Descriptor (15 marks)** — A descriptor class that enforces a value's type on assignment, raising a `TypeError` with a clear message on mismatch. Uses `__set_name__` to auto-derive each attribute's private storage key.

4. **`product_of_multiples` (5 marks)** — A function that returns the product of all multiples of a given factor that fall strictly below a limit.

Each question includes a demo cell showing the solution in action.

## Requirements

- Python 3.10+ (uses `dict[str, list[callable]]` type hint syntax)
- No external libraries — standard library only

## Running it

Open `Assignment1_Answers.ipynb` in Jupyter Notebook, JupyterLab, or VS Code, and run the cells top to bottom.
