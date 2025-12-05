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
Loading seed knowledge from: data/seed_medical.json

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
  Gaps detected: 45
  Questions generated: 45
  Questions pursued: 10
  Questions answered: 5
  Questions blocked: 5
  Duration: 0 ms
  Total questions so far: 10

--- Cycle 2 of 3 ---
✓ Cycle 2 complete!
  Gaps detected: 45
  Questions generated: 45
  Questions pursued: 10
  Questions answered: 5
  Questions blocked: 5
  Duration: 0 ms
  Total questions so far: 20

--- Cycle 3 of 3 ---
✓ Cycle 3 complete!
  Gaps detected: 45
  Questions generated: 45
  Questions pursued: 10
  Questions answered: 5
  Questions blocked: 5
  Duration: 0 ms
  Total questions so far: 30

Summary across all cycles:
  Total gaps detected: 135
  Total questions generated: 135
  Total questions answered: 15

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 12 blocked question(s):

  1. What exactly is clinical trial? [q_2470d04b-812d-41b5-b6b3-7e04f41e2e70]
  2. What exactly is clinical trial? [q_c49f0ac3-e6a5-4131-b748-9c3915f7039c]
  3. What exactly is efficacy? [q_919c327a-88a4-492c-a134-2295ce77617a]
  4. What exactly is clinical trial? [q_02bafdc8-1970-47a8-af67-3f46c72c658f]
  5. What exactly is efficacy? [q_c87ad57a-d54c-495d-9042-ef9bce2cba07]
  ... and 7 more

Press Enter to continue...


─── Step 4: Answering a Question ───
Let's answer the first blocked question:
  Question: What exactly is clinical trial?

  Providing answer: This is a demo answer for: What exactly is clinical trial?

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
  • ece demo --seed data/seed_medical.json --mode basic
  • ece demo --seed data/seed_medical.json --mode interactive
  • ece demo --seed data/seed_medical.json --mode detailed
  • ece demo --seed data/seed_medical.json --mode quick
```