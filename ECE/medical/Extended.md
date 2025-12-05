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
Loading seed knowledge from: data/seed_medical.json

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
  Gaps detected: 45
  Questions generated: 45
  Questions pursued: 10
  Questions answered: 5
  Questions blocked: 5
  Duration: 0 ms

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 4 blocked question(s):

  1. What exactly is clinical trial? [q_7c5489f9-8432-4331-9fc4-6ff5dc489c83]
     Score: 0.755
     Type: Definitional
     Depth: 0
  2. What exactly is efficacy? [q_822d44b0-f751-42a6-ae13-f27c55f2b4f7]
     Score: 0.738
     Type: Definitional
     Depth: 0
  3. What exactly is clinical trial? [q_286a0b1f-5f44-4c8d-8334-047a53872f16]
     Score: 0.755
     Type: Definitional
     Depth: 0
  4. What exactly is efficacy? [q_f800ecfb-2d19-4a0b-b13a-1720b7a365d3]
     Score: 0.738
     Type: Definitional
     Depth: 0

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
  Total questions: 10
  Satisfaction rate: 7%
  Average depth: 0
  Maximum depth: 0
  Knowledge coverage: 5%
  Average concept clarity: 0.

Questions by State:
  Blocked............. 3 (30.0%)
  Satisfied........... 7 (70.0%)

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
  • ece demo --seed data/seed_medical.json --mode basic
  • ece demo --seed data/seed_medical.json --mode extended
  • ece demo --seed data/seed_medical.json --mode interactive
  • ece demo --seed data/seed_medical.json --mode quick
```