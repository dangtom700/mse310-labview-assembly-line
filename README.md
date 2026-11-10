# LabVIEW Assembly-Line Control (MSE 310)

Coursework and final project in LabVIEW: instrument/VI building up to an automated
assembly-line control system with a real-time operator GUI and state persistence
across power loss.

**Course:** MSE 310, Simon Fraser University · **Term:** Sep–Dec 2024 · **Team project**

## What I did

Programmed assembly-line control logic in LabVIEW through calibration and
commissioning, built a real-time GUI for sensor visualisation, and implemented a
power-loss recovery mechanism so the line resumes from its last known state rather
than restarting cold. Architecture and control logic were documented alongside.

This was a team project and **my exact share of it is not yet pinned down** — it is
flagged as an open confirmation in my project ledger. Read the contribution above as
the work I was involved in, not as a sole-author claim.

## What's here

**`MSE 310/`** — individual VIs built through the course:

| File | What it demonstrates |
|---|---|
| `Calculator.vi`, `operation_func.vi` | SubVI composition and arithmetic dataflow |
| `XOR.vi` | Boolean logic primitives |
| `clock gauge.vi` | Front-panel indicator / timing display |
| `Lab Whatever/flat sequence.vi` | Execution-order control via flat sequence |
| `Lab Whatever/enqueue_dequeue.vi` | Queue-based producer/consumer |
| `Lab Whatever/write_then_read.vi` | File I/O round-trip |

**`ProjectMSE310/`** — the final assembly-line project:

| File | What it is |
|---|---|
| `FinalProject.vi` | The delivered control system |
| `FinalProject_alter1.vi`, `AnotherOne.vi` | Earlier design iterations |
| `memory.txt`, `write_memory.txt` | On-disk state files behind the power-loss recovery |
| `rougn_plan.txt` | Working design notes |

`memory.txt` and `write_memory.txt` are the persistence layer that makes the
state-resumption claim above checkable — the line's state is written to disk so a
restart reloads rather than reinitialises.

## Opening these

`.vi` files require **NI LabVIEW**. They are binary and will not render on GitHub;
clone the repo and open them locally. `.txt` files are readable as-is.
