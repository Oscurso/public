```
╔══════════════════════════════════════════════════════════════════════╗
║ STEP 4: LEGAL CONTRACTS ANALYSIS                                     ║
╚══════════════════════════════════════════════════════════════════════╝

Domain: Legal Contracts and Obligations
File: legal_contracts.json (43 concepts, 50 relations)

In this analysis, CDE will examine legal knowledge including:
• Contract terms and obligations
• Legal rights and enforcement mechanisms
• Jurisdictional considerations

Key Expected Findings:
• Contradictions: Conflicting contract clauses
• Edge Cases: Terms that create legal ambiguity
• Assumptions: Unstated legal prerequisites

Press any key to run legal contracts analysis...

Resetting state for clean analysis...

Running CDE analysis...
───────────────────────────────────────────────────────────────────────
═══════════════════════════════════════════════════════════════
  Analyzing knowledge from "data\\legal_contracts.json"
═══════════════════════════════════════════════════════════════

═══════════════════════════════════════════════════════════════
                  CDE ANALYSIS COMPLETE
═══════════════════════════════════════════════════════════════

[ISSUES FOUND]
  Contradictions:     0
  Weak Assumptions:   10
  Edge Cases:         150
  Miscalibrations:    18

[CRITIQUES GENERATED]
  Total:              48
  With Resolutions:   48
  Dialectics Created: 0

  Duration: 0ms

═══════════════════════════════════════════════════════════════
  ACTIVE ISSUES: 20
═══════════════════════════════════════════════════════════════

─────────────────────────────────────────────────────────────
  CRT-8881FE46 | ConfidenceMiscalibration | Severity: 0.54
  State: Active
─────────────────────────────────────────────────────────────
You seem overconfident about 'r_fraud_voidable'. Evidence suggests 42% confidence, not 95%.

─────────────────────────────────────────────────────────────
  CRT-9950DCB1 | ConfidenceMiscalibration | Severity: 0.53
  State: Active
─────────────────────────────────────────────────────────────
You seem overconfident about 'r_minor_voidable'. Evidence suggests 38% confidence, not 90%.

─────────────────────────────────────────────────────────────
  CRT-5C76C50B | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
Where does 'Contracts for necessities valid even with minors' come from? I don't see much backing it up.

─────────────────────────────────────────────────────────────
  CRT-C486A9C9 | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
I question whether 'Oral contracts valid but harder to prove terms' is well-founded. What supports this?

─────────────────────────────────────────────────────────────
  CRT-263949B9 | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
The claim 'Mutual assent plus other elements creates valid contract' seems to be accepted without strong support.

─────────────────────────────────────────────────────────────
  CRT-0F5D4DBB | ConfidenceMiscalibration | Severity: 0.53
  State: Active
─────────────────────────────────────────────────────────────
The 90% confidence on 'r_punitive_damages_rare_contract' feels overconfident. I'd say closer to 38%.

─────────────────────────────────────────────────────────────
  CRT-B5AFC19B | WeakAssumption | Severity: 0.62
  State: Active
─────────────────────────────────────────────────────────────
'Offer requires acceptance to form contract' looks like it's taken for granted. Should we be more cautious here?

─────────────────────────────────────────────────────────────
  CRT-DA728827 | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
'Written contracts provide strong evidence of terms and formation' looks like it's taken for granted. Should we be more cautious here?

─────────────────────────────────────────────────────────────
  CRT-79987D1C | WeakAssumption | Severity: 0.62
  State: Active
─────────────────────────────────────────────────────────────
'Offer plus acceptance creates mutual assent' appears to be an assumption. Has this been verified?

─────────────────────────────────────────────────────────────
  CRT-75C48F18 | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
Where does 'Consideration is essential for valid common law contract' come from? I don't see much backing it up.

─────────────────────────────────────────────────────────────
  CRT-30690F7E | ConfidenceMiscalibration | Severity: 0.52
  State: Active
─────────────────────────────────────────────────────────────
You seem overconfident about 'r_oral_contract_over_500_invalid'. Evidence suggests 38% confidence, not 85%.

─────────────────────────────────────────────────────────────
  CRT-A30F1827 | ConfidenceMiscalibration | Severity: 0.53
  State: Active
─────────────────────────────────────────────────────────────
'r_b2c_consumer_protection' is marked at 90% confidence, but the evidence points to 36%. You're overconfident.

─────────────────────────────────────────────────────────────
  CRT-166F6F3B | WeakAssumption | Severity: 0.60
  State: Active
─────────────────────────────────────────────────────────────
Where does 'Force majeure clause provides contractual excuse for impossibility' come from? I don't see much backing it up.

─────────────────────────────────────────────────────────────
  CRT-D6955412 | ConfidenceMiscalibration | Severity: 0.52
  State: Active
─────────────────────────────────────────────────────────────
I'd adjust confidence in 'r_minor_breach_substantial_performance' from 85% to 36%.

─────────────────────────────────────────────────────────────
  CRT-39DC93B2 | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
'Legal capacity required for valid contract' appears to be an assumption. Has this been verified?

─────────────────────────────────────────────────────────────
  CRT-8754560A | ConfidenceMiscalibration | Severity: 0.54
  State: Active
─────────────────────────────────────────────────────────────
You seem overconfident about 'r_duress_voidable'. Evidence suggests 40% confidence, not 95%.

─────────────────────────────────────────────────────────────
  CRT-D2D400ED | ConfidenceMiscalibration | Severity: 0.52
  State: Active
─────────────────────────────────────────────────────────────
The 85% confidence on 'r_oral_contract_under_500_valid' feels overconfident. I'd say closer to 34%.

─────────────────────────────────────────────────────────────
  CRT-1DEE3804 | ConfidenceMiscalibration | Severity: 0.53
  State: Active
─────────────────────────────────────────────────────────────
You seem overconfident about 'r_voidable_rescission'. Evidence suggests 36% confidence, not 90%.

─────────────────────────────────────────────────────────────
  CRT-353DC62A | ConfidenceMiscalibration | Severity: 0.52
  State: Active
─────────────────────────────────────────────────────────────
'r_undue_influence_voidable' is marked at 90% confidence, but the evidence points to 34%. You're overconfident.

─────────────────────────────────────────────────────────────
  CRT-18CC48EF | WeakAssumption | Severity: 0.61
  State: Active
─────────────────────────────────────────────────────────────
I question whether 'Specific performance typically requires unique subject matter (land, art)' is well-founded. What supports this?



State saved to ".cde_state.json"


[TOP CONTRADICTIONS - Legal Domain]
───────────────────────────────────────────────────────────────────────
═══════════════════════════════════════════════════════════════
  CRITIQUES: 0 found
═══════════════════════════════════════════════════════════════



[TOP WEAK ASSUMPTIONS - Legal Domain]
───────────────────────────────────────────────────────────────────────
═══════════════════════════════════════════════════════════════
  CRITIQUES: 10 found
═══════════════════════════════════════════════════════════════

1. CRT-B5AFC19B [WeakAssumption, severity: 0.62] [Active]
   'Offer requires acceptance to form contract' looks like it's taken for granted. Should we be more cautious here?

2. CRT-79987D1C [WeakAssumption, severity: 0.62] [Active]
   'Offer plus acceptance creates mutual assent' appears to be an assumption. Has this been verified?

3. CRT-18CC48EF [WeakAssumption, severity: 0.61] [Active]
   I question whether 'Specific performance typically requires unique subject matter (land, art)' is well-founded. What supports this?

... and 7 more (use --limit to see more)

Press any key to continue...
```