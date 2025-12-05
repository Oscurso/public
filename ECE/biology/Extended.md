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
Loading seed knowledge from: data/seed_biology.json

✓ Initialization complete!
  Concepts loaded: 18
  Relations loaded: 20

Press Enter to continue...


─── Step 2: Running 3 Curiosity Cycles ───
The ECE will now:
  • Detect knowledge gaps in the concept map
  • Generate questions from those gaps
  • Attempt to pursue and answer questions

--- Cycle 1 of 3 ---
✓ Cycle 1 complete!
  Gaps detected: 28
  Questions generated: 28
  Questions pursued: 10
  Questions answered: 7
  Questions blocked: 3
  Duration: 0 ms
  Total questions so far: 10

--- Cycle 2 of 3 ---
✓ Cycle 2 complete!
  Gaps detected: 28
  Questions generated: 28
  Questions pursued: 10
  Questions answered: 7
  Questions blocked: 3
  Duration: 0 ms
  Total questions so far: 20

--- Cycle 3 of 3 ---
✓ Cycle 3 complete!
  Gaps detected: 28
  Questions generated: 28
  Questions pursued: 10
  Questions answered: 7
  Questions blocked: 3
  Duration: 0 ms
  Total questions so far: 30

Summary across all cycles:
  Total gaps detected: 84
  Total questions generated: 84
  Total questions answered: 21

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 6 blocked question(s):

  1. What exactly is consciousness? [q_da008a21-d2b2-4071-8189-a65eb3466fd5]
  2. What exactly is life? [q_2e3830fe-3dbf-4f16-a12b-6d91206ecd04]
  3. What exactly is consciousness? [q_c2bdf64b-6111-4e1f-9218-b1b78eb3424a]
  4. What exactly is life? [q_e56b086d-25c2-4d2c-bf43-7e8ac7f79adb]
  5. What exactly is life? [q_1d60e971-d6b7-43d5-96f2-1b7c8e4dbb1e]
  ... and 1 more

Press Enter to continue...


─── Step 4: Answering a Question ───
Let's answer the first blocked question:
  Question: What exactly is consciousness?

  Providing answer: This is a demo answer for: What exactly is consciousness?

✓ Answer recorded!
  The question state has been updated to: Satisfied

Press Enter to continue...


─── Step 5: Final Statistics ───
Here's a summary of the current ECE state:

Knowledge Base:
  Concepts: 18
  Relations: 20

Curiosity State:
  Total questions: 30
  Satisfaction rate: 8%
  Average depth: 0

Questions by State:
  Blocked............. 5
  Satisfied........... 25

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
  • ece demo --seed data/seed_biology.json --mode basic
  • ece demo --seed data/seed_biology.json --mode interactive
  • ece demo --seed data/seed_biology.json --mode detailed
  • ece demo --seed data/seed_biology.json --mode quick
```