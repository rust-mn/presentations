---
marp: true
theme: gaia
class: invert
---

# State of GPU Programming in Rust

or

### Getting started with GPU programming in Rust

---

# Outline

- GPU overview
- Memory safety
- GPU crates/projects
- General observations
- Where to learn more

---

# GPU overview

- Good for "embarassingly parallel" problems:
    - easy to divide
    - no communication between tasks
    - no results dependencies between tasks
- Many types of problems can be encoded as "graphics" problems (APIs can help with this)
- GPUs are co-processors!

---

# Memory safety

* CPU memory safety models don't translate to GPUs
* Rust's memory safety model is specific to CPUs
* You can't write "memory safe" Rust for GPUs (_womp, womp_)
* Memory in GPUs is complex and its own topic

---
