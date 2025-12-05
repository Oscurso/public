```
╔══════════════════════════════════════════════════════════════════════╗
║                                                                      ║
║  WIM - WORKING INTENT MEMORY                                         ║
║                                                                      ║
║  Industry Demo: Wedding Planning                                     ║
║  Luxury Event Coordination - Crisis Management                       ║
║                                                                      ║
╚══════════════════════════════════════════════════════════════════════╝

Welcome to the WIM Wedding Planning Demo

This scenario demonstrates how WIM manages the beautiful chaos of
luxury wedding coordination, where vendor crises and emotional clients
require constant context switching without losing critical details.

Role:     Lead Wedding Planner - Luxury Events
Time:     Friday afternoon, 3 weeks before wedding
Location: Active Weddings: 5 concurrent events

Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SCENE 1: Anderson-Chen Wedding - Final Details
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Wedding: Anderson-Chen
Date: December 28, 2024 (23 days away)
Venue: Rosewood Estate Vineyards
Guests: 220 (218 confirmed)
Budget: $145,000

[WIM Operation: wim_intent_create]
▶ Creating primary intent in WIM...

Intent: "Execute Anderson-Chen wedding flawlessly"

[WIM Operation: wim_task_decompose]
Task Progress:
  ✓ WED-FINAL-01: Confirm final headcount
  → WED-FINAL-02: Finalize seating chart [IN PROGRESS - 75%]
  • WED-FINAL-03: Final venue walkthrough
  • WED-FINAL-04: Coordinate day-of timeline (14 vendors)
  • WED-FINAL-05: Final dress fitting

Progress:
[��������������������������������������������������]  20%

▶ Context preserved:

  current task:
    file: anderson_chen_seating_v8.xlsx
    tables finalized: 1-7, 9-15 (14 of 15)
    issue: Table 8 - Aunt Margaret vs Uncle Tom (divorce drama)
    solution: Move Uncle Tom to Table 12 with college friends
    status: Awaiting bride's text approval
  bride stress level: 3
  emotional state: Everything going smoothly


Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SCENE 2: 💐 VENDOR CRISIS ALERT 💐
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━


    ╔═══════════════════════════════════════════════════════════╗
    ║   FLORIST EMERGENCY                                       ║
    ║                                                           ║
    ║   Bella Flora (florist) just CANCELED                     ║
    ║   Owner hospitalized - business temporarily closed        ║
    ║   Time to find replacement: 48 hours                      ║
    ╚═══════════════════════════════════════════════════════════╝

Floral Arrangements Affected:
  • Bridal bouquet (white peonies, garden roses, eucalyptus)
  • 6 bridesmaid bouquets
  • 12 boutonnieres
  • Ceremony arch (3ft × 8ft floral installation)
  • 14 reception centerpieces (tall and low alternating)
  • Cake table, gift table, restroom arrangements
  • Contract value: $8,500

Analyzing urgency...

  Current intent urgency: 0.75
  Interruption urgency:   0.88
  Interruption threshold: 0.80

→ Interruption urgency EXCEEDS threshold
→ Decision: HANDLE_NOW
→ Rationale: Quality florists book fast - 48-hour window critical
WIM Interruption Handler analyzing...

  Current intent urgency: 0.75 (Seating chart - important)
  Interruption urgency:   0.88 (Florist crisis - time-sensitive)
  Interruption threshold: 0.80

→ Vendor crisis EXCEEDS threshold by 0.08
→ Decision: HANDLE IMMEDIATELY - Quality vendors book fast

Bride's stress level: 3/10 → 8/10 (CRISIS MODE)


Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SCENE 3: Context Preservation - Wedding Details
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

[WIM Operation: wim_context_preserve]
WIM is preserving wedding coordination context...

▶ Capturing seating chart state:

  ✓ Spreadsheet: anderson_chen_seating_v8.xlsx
  ✓ Tables 1-7, 9-15 finalized (14/15)
  ✓ Table 8 issue: Aunt Margaret vs Uncle Tom
  ✓ Solution proposed: Move Tom to Table 12
  ✓ Pending: Bride's approval via text

▶ Florist research already started:
  • Backup option 1: Garden of Eden ($9,200 - +$700)
  • Backup option 2: Petal & Stem ($8,800 - +$300)
  • Backup option 3: Moonlight Florals (unavailable - booked)


Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SCENE 4: Florist Crisis Resolution
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Rapid-fire vendor search in progress...

Evaluating replacement florists:

Garden of Eden Florals:
  • Available: ✓
  • Quote: $9,200 (+$700 over original)
  • Style match: 85% - different rose variety needed
  • Can replicate design: Yes, with substitutions

Petal & Stem:
  • Available: ✓
  • Quote: $8,800 (+$300 over original)
  • Style match: 92% - exact match possible
  • Can replicate design: Yes, exact colors and flowers
  • Portfolio: Stunning, bride will love this

→ WIM Decision: Petal & Stem
    Best style match, reasonable price increase, available immediately

Actions completed:
  ✓ Called Petal & Stem (2:47 PM)
  ✓ Sent bride's Pinterest inspo board
  ✓ Received mock-ups (3:15 PM)
  ✓ Bride approved via video call (3:42 PM)
  ✓ Contract signed (4:18 PM)
  ✓ Deposit paid ($3,500)

Crisis resolved in 4 hours

Bride's stress level: 8/10 → 3/10 (RELIEVED!)

"Thank you SO much! I was panicking but you fixed it so fast!"
- Rebecca (bride)


Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SCENE 5: Returning to Seating Chart
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

6:45 PM - Crisis resolved, resuming normal work

▶ WIM restoring seating chart context:

  ✓ Reopened: anderson_chen_seating_v8.xlsx
  ✓ Highlighted: Table 8 (the problem table)
  ✓ Restored note: 'Move Uncle Tom to Table 12 - awaiting approval'
  ✓ Bride's text arrived: 'Yes! Move Tom. Perfect solution!'

▶ Completing seating chart:
  ✓ Uncle Tom moved to Table 12
  ✓ Added college friend group to Table 12
  ✓ Aunt Margaret stays at Table 8 with bride's family
  ✓ Final chart complete (15/15 tables)
  ✓ Sent to venue coordinator
  ✓ Ordered escort cards (calligraphy deadline met)

Progress:
[��������������������������������������������������]  40%

▶ Context restoration time: 1 minute

Without WIM: 15-20 minutes to remember where you were
With WIM: 1 minute - perfect continuity


Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SCENE 6: End-of-Day Report
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━


╔═══════════════════════════════════════════════════════════════════╗
║                    PERFORMANCE METRICS REPORT                     ║
╚═══════════════════════════════════════════════════════════════════╝



  WEDDING: Anderson-Chen (23 days until 'I do')
  CRISIS MANAGEMENT: {"vendor_crisis":"Florist cancellation","time_to_resolution_hours":4,"replacement_quality":"92% style match","budget_impact":"+$300 (2% over - acceptable)","bride_stress_managed":"8/10 → 3/10"}
  TASK COMPLETION: {"seating_chart":"✓ Completed despite crisis","context_switches":3,"details_lost":0,"vendor_coordination":"15 vendors managed simultaneously"}
  CLIENT SATISFACTION: {"response_time_minutes":5,"crisis_confidence":"You saved my wedding!","stress_reduction":"63% (8/10 to 3/10)"}
  TIMELINE PERFORMANCE: {"deadlines_met":"✓ (venue, calligrapher, florist)","days_ahead_of_schedule":3,"contingency_plans":"Weather backup activated"}

Press ENTER to continue...


━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
WIM VALUE PROPOSITION: Wedding Planning
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Why WIM Matters:

Without WIM:
  ✗ 15-20 minutes to remember coordination state
  ✗ Critical details forgotten during crisis (guest allergies, preferences)
  ✗ Client stress escalates without quick responses
  ✗ Average 18 hours to manage vendor crisis
  ✗ Multiple weddings blur together
  ✗ Vendor relationship context lost

With WIM:
  ✓ 1-minute context restoration
  ✓ Zero details lost (guest needs, vendor specs, family dynamics)
  ✓ 4-hour crisis resolution (78% faster)
  ✓ Client stress reduced by 63% through confidence
  ✓ Complete isolation between 5 concurrent weddings
  ✓ Vendor history and preferences automatically recalled

ROI: 156% revenue increase per planner

Press ENTER to continue...
```