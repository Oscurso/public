```
═══════════════════════════════════════════════════════════
    EMERGENT CURIOSITY ENGINE - INTERACTIVE DEMO
═══════════════════════════════════════════════════════════

Mode: Extended
Description: Extended demo with 3 cycles showing question accumulation

This demo will walk you through the core ECE functionality:
  1. Initialize knowledge from a seed file
  2. Run 3 curiosity cycles
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


─── Step 2: Running 3 Curiosity Cycles ───
The ECE will now:
  • Detect knowledge gaps in the concept map
  • Generate questions from those gaps
  • Attempt to pursue and answer questions

--- Cycle 1 of 3 ---
✓ Cycle 1 complete!
  Gaps detected: 41
  Questions generated: 41
  Questions pursued: 10
  Questions answered: 2
  Questions blocked: 8
  Duration: 0 ms
  Total questions so far: 10

--- Cycle 2 of 3 ---
✓ Cycle 2 complete!
  Gaps detected: 41
  Questions generated: 41
  Questions pursued: 10
  Questions answered: 2
  Questions blocked: 8
  Duration: 0 ms
  Total questions so far: 20

--- Cycle 3 of 3 ---
✓ Cycle 3 complete!
  Gaps detected: 41
  Questions generated: 41
  Questions pursued: 10
  Questions answered: 2
  Questions blocked: 8
  Duration: 0 ms
  Total questions so far: 30

Summary across all cycles:
  Total gaps detected: 123
  Total questions generated: 123
  Total questions answered: 6

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 21 blocked question(s):

  1. What exactly is solvency? [q_2e7aa486-6a46-41f2-a85f-3161715aa85b]
  2. What exactly is solvency? [q_d27361e0-957b-4e9e-a024-ba407c1af02b]
  3. What exactly is know your customer? [q_5d634d62-26dd-4aaa-930a-957ec943747c]
  4. What exactly is solvency? [q_bdb7f20d-f732-45f9-ab4d-c1fc7385a32b]
  5. What exactly is creditworthiness? [q_74b8376a-d82a-4255-a7cf-9d22148de62e]
  ... and 16 more

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
  Total questions: 30
  Satisfaction rate: 3%
  Average depth: 0

Questions by State:
  Blocked............. 20
  Satisfied........... 10

Press Enter to continue...


═══════════════════════════════════════════════════════════
                    DEMO COMPLETE!
═══════════════════════════════════════════════════════════

Mode completed: Extended
The ECE state has been saved to: data\ece_state.json

You can now:
  • Run ece cycle to generate more questions
  • Use ece list to view curiosities
  • Run ece stats to see detailed statistics

Try other demo modes:
  • ece demo --seed data/seed_finance.json --mode basic
  • ece demo --seed data/seed_finance.json --mode interactive
  • ece demo --seed data/seed_finance.json --mode detailed
  • ece demo --seed data/seed_finance.json --mode quick
```