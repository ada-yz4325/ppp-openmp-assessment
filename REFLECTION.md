# A1 REFLECTION

> Complete every section. CI will:
>
> 1. Verify all `## Section` headers below are present.
> 2. Verify each section has **at least 50 words**.
>
> No automatic content grading: the prose is read by a human, and the short
> prompt at the end is marked on a 0 / 0.5 / 1 scale. The numbers you quote
> in your reflection do **not** have to match canonical times exactly — HPC
> queue variance is real. Be concise, ground claims in your measurements, show your working.

## Section 1 — Schedule choice and why

Which schedule (`static` / `dynamic` / `guided` / chunk size) did you end up with, and why? Reference the cost structure of `f(x)` and what the measured timings told you. Mention at least one schedule you tried and discarded, and what the measured evidence was. Minimum 50 words.

<!-- your answer here -->

## Section 2 — Scaling behaviour

Looking at your `tables.csv`, where does your speedup curve depart from ideal (linear)? What does that tell you about overhead, memory bandwidth, or load balance for this kernel? Minimum 50 words.

<!-- your answer here -->

## Section 3 — Roofline position

Pick your best thread count. Using the Rome roofline constants from the day-2 slides (theoretical peak 4608 GFLOPs, HPL-achievable 2896 GFLOPs, STREAM triad 246 GB/s), what roofline fraction did you achieve against the *theoretical* and the *HPL-achievable* compute ceilings? Most non-DGEMM code (including A1) lands well below both — explain why your kernel doesn't approach DGEMM-class efficiency. If you want to argue your kernel is bandwidth-bound rather than compute-bound, justify it. Minimum 50 words.

<!-- your answer here -->

## Section 4 — What you'd try next

You have two more days. What would you change about `integrate.cpp`? Pick one concrete change and predict its effect. Minimum 50 words.

<!-- your answer here -->

## Reasoning question (instructor-marked, ≤100 words)

**In at most 100 words, explain why your chosen schedule is appropriate for the cost structure of this particular `f(x)`.**

<!-- your answer here; 100 words max -->
