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
Loading seed knowledge from: data/seed_software.json

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
  Gaps detected: 35
  Questions generated: 35
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms
  Total questions so far: 10

--- Cycle 2 of 3 ---
✓ Cycle 2 complete!
  Gaps detected: 35
  Questions generated: 35
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms
  Total questions so far: 20

--- Cycle 3 of 3 ---
✓ Cycle 3 complete!
  Gaps detected: 35
  Questions generated: 35
  Questions pursued: 10
  Questions answered: 3
  Questions blocked: 7
  Duration: 0 ms
  Total questions so far: 30

Summary across all cycles:
  Total gaps detected: 105
  Total questions generated: 105
  Total questions answered: 9

Press Enter to continue...


─── Step 3: Viewing Blocked Questions ───
Blocked questions are those that couldn't be answered automatically.
These represent true knowledge gaps requiring external input.

Found 15 blocked question(s):

  1. What exactly is scalability? [q_7719f5ce-05d1-42a0-8782-333a0f0cc610]
  2. What exactly is security? [q_10bed91b-5761-4345-8fe4-39d09094cea4]
  3. What exactly is security? [q_787c9c88-6782-4c8a-b199-484fbbc8114c]
  4. What exactly is scalability? [q_caa16d2b-44c7-4ee2-8e3a-20aa7d08b125]
  5. What exactly is scalability? [q_b3f1fd2f-f3cd-43b8-bd02-254bd8c752ad]
  ... and 10 more

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
  Total questions: 30
  Satisfaction rate: 5%
  Average depth: 0

Questions by State:
  Blocked............. 14
  Satisfied........... 16

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
  • ece demo --seed data/seed_software.json --mode basic
  • ece demo --seed data/seed_software.json --mode interactive
  • ece demo --seed data/seed_software.json --mode detailed
  • ece demo --seed data/seed_software.json --mode quick
```