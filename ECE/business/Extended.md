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
Loading seed knowledge from: data/seed_business.json

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
  Gaps detected: 33
  Questions generated: 33
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 4 blocked question(s):

  1. What exactly is competitive moat? [q_3e02f06e-2458-4d96-bf5c-03c39e81b654]
     Score: 0.768
     Type: Definitional
     Depth: 0
  2. What exactly is innovation? [q_02d6c360-3c7d-4fe5-b3da-2a50db65ec0b]
     Score: 0.760
     Type: Definitional
     Depth: 0
  3. What exactly is innovation? [q_c4516f83-576e-494c-b3d0-6cbe60809275]
     Score: 0.760
     Type: Definitional
     Depth: 0
  4. What exactly is competitive moat? [q_7d1c069c-09cf-40bf-874b-1f9baf6eacc3]
     Score: 0.768
     Type: Definitional
     Depth: 0

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
  Total questions: 10
  Satisfaction rate: 7%
  Average depth: 0
  Maximum depth: 0
  Knowledge coverage: 7%
  Average concept clarity: 0.

Questions by State:
  Satisfied........... 7 (70.0%)
  Blocked............. 3 (30.0%)

Gap Analysis:
  Average gaps per cycle: 3
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
  • ece demo --seed data/seed_business.json --mode basic
  • ece demo --seed data/seed_business.json --mode extended
  • ece demo --seed data/seed_business.json --mode interactive
  • ece demo --seed data/seed_business.json --mode quick
```