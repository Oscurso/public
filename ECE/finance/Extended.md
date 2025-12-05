```
═══════════════════════════════════════════════════════════
    EMERGENT CURIOSITY ENGINE - INTERACTIVE DEMO
═══════════════════════════════════════════════════════════

Mode: Detailed
Description: Detailed demo with comprehensive statistics and analysis

This demo will walk you through the core ECE functionality:
  1. Initialize knowledge from a seed file
  2. Run a curiosity cycle
  3. View blocked questions
  4. Answer a question automatically
  5. Review final statistics

Press Enter to continue...


─── Step 1: Initializing ECE ───
Loading seed knowledge from: data/seed_finance.json

✓ Initialization complete!
  Concepts loaded: 20
  Relations loaded: 20

Press Enter to continue...


─── Step 2: Running Curiosity Cycle ───
The ECE will now:
  • Detect knowledge gaps in the concept map
  • Generate questions from those gaps
  • Attempt to pursue and answer questions

✓ Cycle 1 complete!
  Gaps detected: 41
  Questions generated: 41
  Questions pursued: 10
  Questions answered: 2
  Questions blocked: 8
  Duration: 0 ms

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 7 blocked question(s):

  1. What exactly is solvency? [q_c6c38098-195f-40d0-b9cb-e362cbb91f7f]
     Score: 0.759
     Type: Definitional
     Depth: 0
  2. What exactly is know your customer? [q_9677154f-012f-4daf-9926-935493e29753]
     Score: 0.740
     Type: Definitional
     Depth: 0
  3. What exactly is creditworthiness? [q_356e7001-fb77-44ff-9158-407b6aa519f8]
     Score: 0.580
     Type: Definitional
     Depth: 0
  4. What exactly is fraud? [q_888fc18d-a6fa-4602-a903-ad54496d7c2c]
     Score: 0.733
     Type: Definitional
     Depth: 0
  5. What exactly is creditworthiness? [q_50fa6e32-0bb8-4091-b052-102d6405becb]
     Score: 0.580
     Type: Definitional
     Depth: 0
  6. What exactly is solvency? [q_d7cc2bce-6310-4c4c-9b01-62d61a119e2a]
     Score: 0.759
     Type: Definitional
     Depth: 0
  7. What exactly is know your customer? [q_40404103-6bde-403c-ae56-46ccd1b78e95]
     Score: 0.740
     Type: Definitional
     Depth: 0

Press Enter to continue...


─── Step 4: Answering a Question ───
Let's answer the first blocked question:
  Question: What exactly is solvency?

  Providing answer: This is a demo answer for: What exactly is solvency?

✓ Answer recorded!
  The question state has been updated to: Satisfied

Press Enter to continue...


─── Step 5: Final Statistics ───
Here's a summary of the current ECE state:

Knowledge Base:
  Concepts: 20
  Relations: 20

Curiosity State:
  Total questions: 10
  Satisfaction rate: 4%
  Average depth: 0
  Maximum depth: 0
  Knowledge coverage: 6%
  Average concept clarity: 0.

Questions by State:
  Satisfied........... 4 (40.0%)
  Blocked............. 6 (60.0%)

Gap Analysis:
  Average gaps per cycle: 4
  Gap-to-question ratio: 1

Press Enter to continue...


═══════════════════════════════════════════════════════════
                    DEMO COMPLETE!
═══════════════════════════════════════════════════════════

Mode completed: Detailed
The ECE state has been saved to: data\ece_state.json

You can now:
  • Run ece cycle to generate more questions
  • Use ece list to view curiosities
  • Run ece stats to see detailed statistics

Try other demo modes:
  • ece demo --seed data/seed_finance.json --mode basic
  • ece demo --seed data/seed_finance.json --mode extended
  • ece demo --seed data/seed_finance.json --mode interactive
  • ece demo --seed data/seed_finance.json --mode quick
```