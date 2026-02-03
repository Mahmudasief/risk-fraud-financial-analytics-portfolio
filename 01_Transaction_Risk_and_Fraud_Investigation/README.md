# Case 1: Transaction Risk & Fraud Investigation

## Case Snapshot

**Domain:** Transaction Monitoring & Fraud Investigation  
**Tools:** Excel (analyst workpapers), structured alert review, written investigation summary  
**Focus:** Judgment-based alert triage, escalation vs. clearance decisions, false positive control  

**What this case demonstrates:**
- How transaction alerts are evaluated using risk indicators rather than raw rule triggers
- How analysts distinguish true risk from false positives
- How escalation decisions are documented in a defensible, regulator-ready manner
- How investigation outputs feed downstream risk scoring and escalation models (Case 2)

---

## Objective

The objective of this case is to simulate real-world transaction monitoring and alert investigation for a business checking account, focusing on:

- Identifying meaningful risk signals within noisy transaction data  
- Applying analyst judgment to escalate or clear alerts  
- Reducing false positives while maintaining adequate risk coverage  

This case reflects how frontline fraud and AML analysts operate in production environments — balancing detection accuracy, regulatory expectations, and operational efficiency.

---

## Investigation Framework

Each alert is reviewed using a structured investigation framework:

1. **Alert Intake**
   - Review triggered alerts generated from transaction activity
   - Assess alert context rather than treating rule hits as automatic risk

2. **Risk Indicator Assessment**
   Transactions are evaluated across multiple dimensions, including:
   - Transaction velocity and frequency
   - Structuring or pass-through behavior
   - Unusual transaction amounts relative to customer profile
   - Offshore or higher-risk jurisdiction exposure

3. **Judgment-Based Decisioning**
   - Alerts are **not automatically escalated**
   - Analyst judgment is applied to determine whether behavior is explainable or anomalous

4. **Disposition Outcome**
   - **Escalate** → behavior warrants further review or reporting
   - **Clear** → activity deemed non-suspicious with documented rationale

---

## Escalation & Clearance Logic

This case explicitly contrasts **judgment-based escalation** with mechanical rule-based decisioning.

### Escalation occurs when:
- Multiple risk indicators reinforce each other
- Transaction behavior deviates meaningfully from expected patterns
- Activity cannot be reasonably explained by customer profile or business purpose

### Clearance occurs when:
- Alerts are driven by benign business activity
- Apparent anomalies are explainable and consistent
- No sustained or compounding risk patterns are observed

This approach reflects how effective monitoring programs reduce false positives without weakening risk controls.

---

## Analyst Workpapers

The investigation is documented using structured Excel-based analyst workpapers that capture:

- Transaction-level observations  
- Identified risk indicators  
- Analyst reasoning and conclusions  
- Escalation or clearance decision with justification  

This documentation mirrors real compliance environments where decisions must be **auditable, defensible, and regulator-ready**.

---

## Investigation Summary

A one-page written investigation summary consolidates findings, including:

- Key behaviors observed  
- Risk indicators considered  
- Final disposition decision  
- Rationale supporting escalation or clearance  

This simulates professional case narratives used in fraud investigations and SAR preparation workflows.

---

## Key Insights

- Not all alert triggers indicate true risk — context matters
- Transaction velocity and structuring behavior are stronger risk signals than isolated events
- Judgment-based review significantly reduces false positives
- Clear documentation is critical for defensibility and downstream decisioning

---

## Why This Matters

In real fraud and AML operations:

- Excessive false positives overwhelm analysts
- Poor documentation weakens regulatory defensibility
- Escalation decisions must be explainable, not just rule-driven  

This case demonstrates how **frontline investigation quality directly impacts escalation efficiency, analyst workload, and compliance outcomes**.

---

## Portfolio Context

This case represents the **investigation and alert-review layer** of the financial crime analytics lifecycle.

Its outputs feed directly into:

- **Case 2: Risk Scoring & Operational Analytics**  
  where investigation insights are transformed into:
  - Composite risk scores
  - Escalation thresholds
  - Analyst capacity planning models

Together, these cases illustrate the **end-to-end financial crime workflow**:  
**transaction review → investigation → risk scoring → operational decision support**.

---

## Deliverables

- `transactions.csv` — synthetic transaction dataset  
- `Case1_Analyst_Workpaper.xlsx` — structured alert review and disposition  
- `Case1_Investigation_Summary.pdf` — written investigation narrative  
