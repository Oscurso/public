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
Loading seed knowledge from: data/seed_biology.json

✓ Initialization complete!
  Concepts loaded: 18
  Relations loaded: 20

Press Enter to continue...


─── Step 2: Running Curiosity Cycle ───
The ECE will now:
  • Detect knowledge gaps in the concept map
  • Generate questions from those gaps
  • Attempt to pursue and answer questions

✓ Cycle 1 complete!
  Gaps detected: 28
  Questions generated: 28
  Questions pursued: 10
  Questions answered: 7
  Questions blocked: 3
  Duration: 0 ms

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 2 blocked question(s):

  1. What exactly is life? [q_d9297b06-7f5d-42ca-b8ef-c2428fc9372f]
     Score: 0.564
     Type: Definitional
     Depth: 0
  2. What exactly is consciousness? [q_e16ddff1-6dd5-4746-baa1-786591319c02]
     Score: 0.557
     Type: Definitional
     Depth: 0

Press Enter to continue...


─── Step 4: Answering a Question ───
Let's answer the first blocked question:
  Question: What exactly is life?

  Providing answer: This is a demo answer for: What exactly is life?

✓ Answer recorded!
  The question state has been updated to: Satisfied

Press Enter to continue...


─── Step 5: Final Statistics ───
Here's a summary of the current ECE state:

Knowledge Base:
  Concepts: 18
  Relations: 20

Curiosity State:
  Total questions: 10
  Satisfaction rate: 9%
  Average depth: 0
  Maximum depth: 0
  Knowledge coverage: 7%
  Average concept clarity: 0.

Questions by State:
  Blocked............. 1 (10.0%)
  Satisfied........... 9 (90.0%)

Gap Analysis:
  Average gaps per cycle: 2
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
  • ece demo --seed data/seed_biology.json --mode basic
  • ece demo --seed data/seed_biology.json --mode extended
  • ece demo --seed data/seed_biology.json --mode interactive
  • ece demo --seed data/seed_biology.json --mode quick
```