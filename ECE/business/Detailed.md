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
Loading seed knowledge from: data/seed_business.json

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
  Gaps detected: 33
  Questions generated: 33
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms
  Total questions so far: 10

--- Cycle 2 of 3 ---
✓ Cycle 2 complete!
  Gaps detected: 33
  Questions generated: 33
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms
  Total questions so far: 20

--- Cycle 3 of 3 ---
✓ Cycle 3 complete!
  Gaps detected: 33
  Questions generated: 33
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms
  Total questions so far: 30

Summary across all cycles:
  Total gaps detected: 99
  Total questions generated: 99
  Total questions answered: 9

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 12 blocked question(s):

  1. What exactly is competitive moat? [q_004b2142-16bd-4547-980e-30d987cf4639]
  2. What exactly is innovation? [q_6db69249-58e4-4df4-b27b-d8bb57e0ed8b]
  3. What exactly is innovation? [q_030dc938-1714-413a-8941-4aac1862301b]
  4. What exactly is innovation? [q_98a99c14-539f-4b16-ac09-2afb3201c224]
  5. What exactly is innovation? [q_6eaddbf0-d57b-4918-8f31-9dacdbe43f28]
  ... and 7 more

Press Enter to continue...


─── Step 4: Answering a Question ───
Let's answer the first blocked question:
  Question: What exactly is competitive moat?

  Providing answer: This is a demo answer for: What exactly is competitive moat?

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
  Satisfaction rate: 6%
  Average depth: 0

Questions by State:
  Blocked............. 11
  Satisfied........... 19

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
  • ece demo --seed data/seed_business.json --mode basic
  • ece demo --seed data/seed_business.json --mode interactive
  • ece demo --seed data/seed_business.json --mode detailed
  • ece demo --seed data/seed_business.json --mode quick
```