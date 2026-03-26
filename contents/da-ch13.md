\newpage

## Section 10: Homework Assignment – Data Transformation Challenge

This assignment brings together all the advanced Python tools you’ve learned in
this chapter. You’ll work with a dataset and apply transformations using
comprehensions, lambda functions, built-in functions, and clean Pythonic
patterns.

---

### Dataset

Use the following dataset of airplanes:

```python
planes = [
    {"name": "F-16", "type": "fighter", "range": 4220},
    {"name": "Boeing 737", "type": "passenger", "range": 5600},
    {"name": "A-10", "type": "attack", "range": 4150},
    {"name": "F-22", "type": "fighter", "range": 2960},
    {"name": "Cessna 172", "type": "passenger", "range": 1285},
    {"name": "B-2 Spirit", "type": "bomber", "range": 11100}
]
```

---

## Part 1 – Filtering and Transformation

1. Create a list of all airplane names.
2. Create a list of airplane names where the range is greater than 4000 km.
3. Create a list of ranges for only passenger planes.

> Requirement: Use at least one **list comprehension**.

---

## Part 2 – Sorting with Lambda

1. Sort the airplanes by range (smallest to largest).
2. Sort the airplanes by name (alphabetically).
3. Sort the airplanes by range (largest to smallest).

> Requirement: Use `sorted()` with a **lambda function**.

---

## Part 3 – Dictionary Construction

1. Create a dictionary mapping airplane name → range.
2. Create a dictionary mapping airplane name → type (only include planes with range > 4000).

> Requirement: Use at least one **dictionary comprehension**.

---

## Part 4 – Built-in Functions

1. Find the airplane with the maximum range.
2. Find the airplane with the minimum range.
3. Calculate the total range of all airplanes.
4. Check if any airplane has a range less than 1500.
5. Check if all airplanes have a range greater than 1000.

> Requirement: Use built-in functions such as `max()`, `min()`, `sum()`, `any()`, `all()`.

---

## Part 5 – Combining Techniques

1. Create a sorted list of airplane names where:

   * The range is greater than 3000
   * The result is sorted alphabetically

2. Create a list of types (no duplicates).

> Requirement: Combine multiple techniques (comprehension + built-ins + lambda).

---

## Challenge (Optional)

1. Group airplanes by type into a dictionary:

   ```python
   {
       "fighter": [...],
       "passenger": [...],
       ...
   }
   ```

2. Find the average range of all airplanes.

3. Write a function that returns all airplane names above a given range threshold.

---

### Submission Requirements

* Submit a single `.py` file
* Clearly label each part using comments
* Use clean, readable, Pythonic code
* Avoid unnecessary loops if a better approach exists

---

> **Helpful Hint:**
> Before writing a loop, ask yourself:
>
> * Can this be done with a comprehension?
> * Is there a built-in function that already solves this?

---

### Final Thought

This assignment mirrors real-world data processing tasks. The same patterns you
used here are used in:

* APIs
* Database queries
* Data pipelines
* Backend services

Master these patterns, and you’ll write faster, cleaner, and more professional Python code.