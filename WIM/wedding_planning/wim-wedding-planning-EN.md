# WIM - Working Intent Memory

## Wedding Planning Application

### What is WIM?

WIM is a cognitive module that manages **intent tracking and context preservation** in high-stakes environments. It answers the question: "What am I doing and why?"

**Core Principle:** In luxury wedding coordination where vendor crises and emotional clients require constant context switching, WIM ensures that no critical detail is lost and that you can manage multiple weddings simultaneously without confusion.

---

## How Does It Work?

1. **Intent Creation** - Wedding goals registered with dates and priorities
2. **Task Decomposition** - Complex events broken into trackable milestones
3. **Focus Management** - Tracks current wedding and task context
4. **Interruption Handling** - Evaluates vendor crises: handle now or defer?
5. **Context Preservation** - Captures complete wedding state (seating, vendors, client preferences)
6. **Progress Tracking** - Monitors completion across multiple concurrent weddings

---

## Wedding Planning Scenario

### The Challenge

A lead wedding planner managing 5 concurrent luxury events. Deep in seating chart details for a $145,000 wedding when the florist cancels - owner hospitalized, business closed, 23 days until the wedding. How do you:

- Respond to the vendor crisis without losing your seating chart work?
- Preserve all the context about family dynamics and table arrangements?
- Find a replacement florist that matches the bride's vision?
- Keep the bride calm while resolving a major crisis?

### WIM in Action

| Time | Event | WIM Response |
|------|-------|--------------|
| 14:00 | Seating chart work | Creates intent, tracks Table 8 family drama |
| 14:30 | 75% complete | Aunt Margaret vs Uncle Tom issue being solved |
| 14:45 | FLORIST CANCELS | Evaluates urgency: 0.88 vs threshold 0.80 |
| 14:45 | Decision | HANDLE_NOW - quality vendors book fast |
| 14:47 | Context preserved | Seating state saved, switches to vendor search |
| 18:18 | New florist signed | Petal & Stem, 92% style match, +$300 |
| 18:45 | Return to seating | Restores context in 1 minute |
| 19:00 | Seating complete | All 15 tables finalized, escort cards ordered |

---

## Demo Results

### Vendor Crisis Analysis

```
Current intent urgency:   0.75 (Seating chart - important)
Interruption urgency:     0.88 (Florist crisis - time-sensitive)
Interruption threshold:   0.80

→ Vendor crisis EXCEEDS threshold by 0.08
→ Decision: HANDLE IMMEDIATELY
→ Rationale: Quality vendors book fast - 48-hour window critical
```

WIM understands wedding reality - when a key vendor cancels 3 weeks out, every hour counts. The decision to pause seating work is automatic and justified.

### Wedding Context Preservation

When switching to crisis mode, WIM captured:

- **Spreadsheet state:** anderson_chen_seating_v8.xlsx
- **Tables finalized:** 1-7, 9-15 (14 of 15 complete)
- **Problem table:** Table 8 - Aunt Margaret vs Uncle Tom (divorce drama)
- **Proposed solution:** Move Uncle Tom to Table 12 with college friends
- **Pending approval:** Awaiting bride's text
- **Bride stress level:** 3/10 (was calm before crisis)

**Context restoration time: 1 minute** (vs 15-20 minutes without WIM)

### Crisis Resolution

**Florist replacement process:**

| Vendor | Available | Quote | Style Match | Decision |
|--------|-----------|-------|-------------|----------|
| Garden of Eden | ✓ | $9,200 (+$700) | 85% | Backup |
| Petal & Stem | ✓ | $8,800 (+$300) | 92% | **Selected** |
| Moonlight Florals | ✗ | - | - | Booked |

**Timeline:**
- 14:47 - Called Petal & Stem
- 15:15 - Received mock-ups
- 15:42 - Bride approved via video call
- 16:18 - Contract signed, deposit paid

**Crisis resolved in 4 hours** (industry average: 18 hours)

**Bride stress level: 8/10 → 3/10** ("You saved my wedding!")

---

## Performance Metrics

### End-of-Day Summary

| Metric | Value |
|--------|-------|
| Wedding | Anderson-Chen (23 days out) |
| Vendor Crisis | Florist cancellation |
| Time to Resolution | 4 hours |
| Replacement Quality | 92% style match |
| Budget Impact | +$300 (2% over - acceptable) |
| Seating Chart | ✓ Completed despite crisis |
| Context Switches | 3 |
| Details Lost | 0 |
| Vendors Managed | 15 simultaneously |
| Response Time | 5 minutes |
| Client Stress Reduction | 63% (8/10 → 3/10) |
| Deadlines Met | All (venue, calligrapher, florist) |
| Days Ahead of Schedule | 3 |

---

## Why WIM Matters in Wedding Planning

### Without WIM

- ✗ 15-20 minutes to remember coordination state
- ✗ Critical details forgotten during crisis (guest allergies, preferences)
- ✗ Client stress escalates without quick responses
- ✗ Average 18 hours to manage vendor crisis
- ✗ Multiple weddings blur together
- ✗ Vendor relationship context lost
- ✗ "Wait, which wedding was the peony allergy?"

### With WIM

- ✓ 1-minute context restoration
- ✓ Zero details lost (guest needs, vendor specs, family dynamics)
- ✓ 4-hour crisis resolution (78% faster)
- ✓ Client stress reduced by 63% through confidence
- ✓ Complete isolation between 5 concurrent weddings
- ✓ Vendor history and preferences automatically recalled
- ✓ "The Aunt Margaret situation - I remember exactly"

---

## ROI Calculation

**Per Planner: 156% revenue increase**

Based on:
- Handle 5 concurrent weddings vs 3 (67% capacity increase)
- 78% faster crisis resolution = more time for client service
- Higher client satisfaction = more referrals (wedding industry is 80% referral)
- Zero detail loss = no costly mistakes (wrong flowers, seating disasters)
- Premium pricing justified by reliability and responsiveness

**Example:**
- Before WIM: 12 weddings/year × $8,000 avg fee = $96,000
- With WIM: 20 weddings/year × $12,000 avg fee = $240,000
- Increase: $144,000 (150% revenue growth)

---

## Why This Is Different From Wedding Planning Software

| Aspect | Traditional Software (Aisle Planner, HoneyBook) | WIM |
|--------|------------------------------------------------|-----|
| Focus | Checklist and timeline | Intent and context management |
| Family dynamics | Notes field | Active tracking with solutions |
| Vendor crisis | Manual scramble | Automatic prioritization |
| Context switching | Start over each time | 1-minute complete restoration |
| Multiple weddings | Separate dashboards | Unified with complete isolation |
| Client emotional state | Not tracked | Stress level monitoring |
| Mental context | Lost | "Move Tom to Table 12" preserved |

---

## Technical Specifications

- **Language:** Rust
- **Binary:** `wim` (standalone executable, cross-platform)
- **State format:** JSON
- **Input:** Knowledge-driven scenarios
- **Output:** CLI + JSON + Reports
- **Integration:** ICS-ready for full cognitive stack

---

## Target Users

- **Wedding Planners** - Independent and agency planners
- **Event Coordinators** - Corporate and social events
- **Venue Managers** - Multi-event coordination
- **Catering Directors** - Complex event logistics
- **Destination Wedding Specialists** - Remote coordination
- **Day-of Coordinators** - Crisis management focus

---

## Client Relationship Benefits

WIM helps maintain:

- **Trust** - Never forget a client preference
- **Responsiveness** - 5-minute crisis response time
- **Professionalism** - Seamless context switching
- **Calm** - Client stress management through confidence
- **Accuracy** - Zero detail loss across complex events
- **Referrals** - "She remembered everything about our wedding"

---

## Next Steps

1. **ICS Integration** - Connect with ECE, RSIR, CDE for complete cognitive loop
2. **Vendor Database** - Automatic backup vendor suggestions
3. **Client Portal** - Real-time progress sharing
4. **Budget Tracking** - Live financial impact analysis
5. **Timeline Sync** - Vendor coordination automation

---

## Contact

Oscurso Labs
https://oscurso.com
