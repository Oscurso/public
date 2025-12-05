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
Loading seed knowledge from: data/seed_software.json

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
  Gaps detected: 35
  Questions generated: 35
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 5 blocked question(s):

  1. What exactly is scalability? [q_3d92cd6e-e31d-4f24-9f84-fbc666575b4e]
     Score: 0.750
     Type: Definitional
     Depth: 0
  2. What exactly is security? [q_136e4ab9-cdf6-49ac-afb6-6c438ca3ed0d]
     Score: 0.730
     Type: Definitional
     Depth: 0
  3. What exactly is security? [q_336f0f7f-43ce-48e0-b9ad-16b1b11e6494]
     Score: 0.730
     Type: Definitional
     Depth: 0
  4. What exactly is scalability? [q_4756e4b1-66a8-417c-92db-b97f6d8a7c19]
     Score: 0.750
     Type: Definitional
     Depth: 0
  5. What exactly is maintainability? [q_a52f68b5-c4a8-4e36-988d-63ed472d3959]
     Score: 0.736
     Type: Definitional
     Depth: 0

Press Enter to continue...


─── Step 4: Answering a Question ───
Let's answer the first blocked question:
  Question: What exactly is scalability?

  Providing answer: This is a demo answer for: What exactly is scalability?

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
  Satisfaction rate: 6%
  Average depth: 0
  Maximum depth: 0
  Knowledge coverage: 6%
  Average concept clarity: 0.

Questions by State:
  Blocked............. 4 (40.0%)
  Satisfied........... 6 (60.0%)

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
  • ece demo --seed data/seed_software.json --mode basic
  • ece demo --seed data/seed_software.json --mode extended
  • ece demo --seed data/seed_software.json --mode interactive
  • ece demo --seed data/seed_software.json --mode quick
```