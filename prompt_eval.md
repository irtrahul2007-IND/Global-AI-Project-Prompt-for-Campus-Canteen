# AI Prompt Evaluation Report

**Target Prompt File:** [`college-canteen-quickprompt-enhanced.md`](file:///c:/Users/rahul/OneDrive/Desktop/Campus%20Food%20Prompt/college-canteen-quickprompt-enhanced.md)  
**Evaluation Date:** 2026-09-26  
**Evaluator:** Antigravity AI Prompt Evaluator  

---

## 1. Overall Score Summary

| # | Evaluation Parameter | Maximum Marks | Awarded Score | Percentage |
|---|---|---|---|---|
| 1 | **Prompt Clarity** | 100 | **94** | 94.0% |
| 2 | **Output Quality & Schema Guidance** | 100 | **79** | 79.0% |
| 3 | **Efficiency & Token Economy** | 50 | **43** | 86.0% |
| | **TOTAL SCORE** | **250** | **216** | **86.4%** |

```
Overall Rating: [████████████████░░░] 216 / 250 (86.4% - Grade A / Production Quality)
```

---

## 2. Executive Summary

[`college-canteen-quickprompt-enhanced.md`](file:///c:/Users/rahul/OneDrive/Desktop/Campus%20Food%20Prompt/college-canteen-quickprompt-enhanced.md) is an exceptionally structured, highly detailed, and domain-grounded prompt designed to generate a 7-day college canteen turnaround blueprint. 

### Key Strengths:
1. **Exceptional Domain & Persona Grounding:** Combines multi-disciplinary personas (food-service operations consultant, micro-budget financial strategist, growth hacker, resilient operator) with concrete Indian campus operational realities (₹10,000 budget, 15-minute rush windows, ingredient cross-utilization).
2. **Explicit Mathematical & Contingency Boundaries:** Mandates rigorous unit economics, day-parting demand shifts, zero-waste repurposing, and quantitative failure-mode thresholds (e.g., Day 2 <40% sell-through triggers item withdrawal).

### Primary Areas for Improvement:
1. **Lack of In-Context Few-Shot Demonstrations:** Does not provide full exemplar tables showing target calculations and formats.
2. **Dynamic Parameterization:** Hardcodes variables (₹10,000, 7 days, Indian Rupee) without generic variable slots (e.g., `{{budget}}`, `{{timeline}}`), reducing automated pipeline reusability.
3. **Absence of Modern XML Structural Delimiters:** Relies on Markdown headers rather than structured XML encapsulation (`<system_instructions>`, `<constraints>`, `<deliverables>`, `<output_format>`).

---

## 3. Evaluated Prompt Analysis

- **Target File:** [`college-canteen-quickprompt-enhanced.md`](file:///c:/Users/rahul/OneDrive/Desktop/Campus%20Food%20Prompt/college-canteen-quickprompt-enhanced.md)
- **Estimated Token Count:** ~960 tokens (~7,068 characters)
- **Primary Domain:** Campus Enterprise / Food-Service Operations / Micro-Budget Strategy
- **Structural Organization:** 6 Major Sections (`ROLE & OBJECTIVE`, `CONSTRAINTS & OPERATIONAL PARAMETERS`, `ASSUMPTIONS TO STATE UP FRONT`, `CORE DELIVERABLES REQUIRED` [7 Sub-Deliverables], `TONE & PRESENTATION RULES`, `FINAL OUTPUT STRUCTURE`).

---

## 4. Detailed Parameter Breakdown

### Parameter 1: Prompt Clarity (Awarded: 94 / 100)

| Sub-Criterion | Max Marks | Awarded | Rationale & Evidence |
|---|---|---|---|
| **Role & Persona Definition** | 20 | **19** | *Strength:* Multi-dimensional identity defined upfront: *"elite food-service operations consultant, micro-budget financial strategist, and university campus enterprise specialist... zero-budget campus growth-hacker... resilient operator"* (Lines 1–2). Sets clear mental models and strategic perspective. |
| **Task Specificity & Negative Constraints** | 25 | **24** | *Strength:* Highly specific sub-tasks across 7 key operational areas. Clear negative constraints: *"never guess silently"*, *"no heavy capital expenditure"*, *"no placeholder values, no skipped sections"* (Lines 10, 15, 74). |
| **Instruction Structure & Delimiters** | 20 | **17** | *Strength:* Clean Markdown hierarchy and horizontal dividers (`---`).<br>*Weakness:* Lacks semantic XML boundaries (e.g. `<rules>`, `<schema>`) which improve attention steering in modern LLMs. |
| **Tone, Style & Target Audience** | 15 | **15** | *Strength:* Explicit tone instructions: *"Deliver actionable, data-driven operational guidelines rather than generic advice. Use explicit rupee figures, quantities, and realistic Indian campus food market pricing"* (Lines 66–67). |
| **Unambiguous Language** | 20 | **19** | *Strength:* Direct, deterministic mandates with strict metrics (₹10,000 ceiling, 45–60 sec order fulfillment, 10% contingency buffer, 15% wastage trigger). |

---

### Parameter 2: Output Quality & Schema Compliance (Awarded: 79 / 100)

| Sub-Criterion | Max Marks | Awarded | Rationale & Evidence |
|---|---|---|---|
| **Output Format & Schema Enforcement** | 30 | **26** | *Strength:* Explicitly defines markdown output order (Deliverables 1–7 in order), markdown headings, and specifies table column headers for Unit Economics (Line 25) and Capital Allocation (Lines 26–30).<br>*Weakness:* Does not mandate a strict table schema for Day-by-Day Cash Flows (Deliverable 4) or the Contingency Playbook (Deliverable 7). |
| **Few-Shot Examples & Demonstrations** | 25 | **14** | *Strength:* Contains mini inline references (e.g., *"leftover bread + potato filling → a next-morning sandwich special"*, *"bring a friend who hasn't ordered yet, both get ₹5 off"*).<br>*Weakness:* Lacks complete input-output few-shot demonstrations showing exactly how the mathematical financial table and day-parting schedule should look. |
| **Edge Cases & Fallback Instructions** | 25 | **20** | *Strength:* Exceptional operational edge case handling built into Deliverable 7 (item flops, rain/exam footfall shocks, ingredient price spikes).<br>*Weakness:* Lacks system-level instructions on what to do if user inputs are contradictory or if critical canteen variables are missing. |
| **Factuality & Hallucination Prevention** | 20 | **19** | *Strength:* Mandates stating all assumptions up front: *"every downstream number in the plan should be traceable back to one of these stated assumptions"* and *"no placeholder values"* (Lines 15, 74). |

---

### Parameter 3: Efficiency & Token Economy (Awarded: 43 / 50)

| Sub-Criterion | Max Marks | Awarded | Rationale & Evidence |
|---|---|---|---|
| **Conciseness & Fluff Elimination** | 15 | **14** | *Strength:* Minimal fluff. Every sentence introduces constraints, domain mechanics, or formatting directives. |
| **Token Economy & Context Footprint** | 15 | **14** | *Strength:* High information density; covers operations, finance, menu engineering, queue theory, and marketing in <1,000 tokens. |
| **Dynamic Parameterization** | 10 | **6** | *Weakness:* Values like ₹10,000, 7 days, and Indian context are hard-coded directly instead of parameterized with template tags (`{{working_capital}}`, `{{currency_symbol}}`, `{{duration_days}}`, `{{campus_context}}`). |
| **Signal-to-Noise Ratio** | 10 | **9** | *Strength:* Strong logical ordering: Persona → Constraints → Assumptions → 7 Core Deliverables → Rules → Output Structure. |

---

## 5. Actionable Recommendations

1. **Implement XML Structural Encapsulation:** Wrap the prompt into standardized XML tags (`<system_role>`, `<context_variables>`, `<constraints>`, `<deliverables>`, `<output_format>`) to prevent prompt drift and optimize LLM attention.
2. **Add Parameterized Template Placeholders:** Introduce variable slots like `{{WORKING_CAPITAL}}`, `{{TIMELINE_DAYS}}`, `{{CAMPUS_PROFILE}}` so the prompt can be reused across different campus scenarios.
3. **Standardize Complete Table Schemas:** Provide explicit markdown table schemas for Deliverable 4 (7-Day Cash Flow) and Deliverable 7 (Contingency Matrix) alongside Deliverable 1.
4. **Include a Concrete Few-Shot Golden Example:** Embed a brief, high-fidelity sample row showing realistic unit economics and margin calculations.

---

## 6. Optimized Production-Ready Rewrite

Below is the fully refactored, enterprise-grade prompt incorporating XML structure, parameterization, strict schema enforcement, and few-shot formatting.

```markdown
<system_role>
You are an elite food-service operations consultant, micro-budget financial strategist, university enterprise specialist, and zero-budget campus growth hacker. Your objective is to formulate a high-throughput, operationally robust, and financially self-sustaining turnaround blueprint for a campus canteen.
</system_role>

<operational_parameters>
- Working Capital Ceiling: {{WORKING_CAPITAL|default:"₹10,000"}}
- Execution Window: {{TIMELINE_DAYS|default:"7 Days"}} (5 Academic Peak Days + 2 Prep/Low-Traffic Days)
- Currency: {{CURRENCY|default:"INR (₹)"}}
- Service Target: Under 60 seconds per transaction
- Break Duration: 15-minute inter-class peak windows
- Operating Constraints: Limited cold storage, zero heavy CapEx, high perishable risk
</operational_parameters>

<rules_and_constraints>
1. GROUNDING & TRACEABILITY: State all baseline assumptions (daily footfall, conversion %, competitor pricing) in Section 1. Every downstream calculation must mathematically derive from these assumptions.
2. NO PLACEHOLDERS: Populate all tables with realistic market figures. Never output "[Insert item]", "TBD", or hypothetical blanks.
3. ZERO-BUDGET MARKETING: Rely exclusively on zero-cost organic campus channels (CR WhatsApp broadcasts, referral mechanics).
4. INGREDIENT CROSS-UTILIZATION: Maintain a maximum of 4–5 core SKUs utilizing shared base ingredients.
5. FINANCIAL DISCIPLINE: Enforce a minimum 10% contingency cash reserve at all times.
</rules_and_constraints>

<deliverables_specification>

### Deliverable 1: Explicit Baseline Assumptions & Capital Allocation
- State baseline footfall, conversion rate, exam/rain factors, and competitor price anchors.
- Provide initial capital allocation breakdown table:
  | Budget Category | Allocated Amount (₹) | % of Total Capital | Justification & Purpose |
  |---|---|---|---|
  | Raw Ingredients / Inventory | | | |
  | Packaging & Disposables | | | |
  | Operations / Marketing | | | |
  | Emergency Contingency Buffer | | | Minimum 10% required |
  | **TOTAL** | **₹10,000** | **100%** | |

### Deliverable 2: High-Throughput Menu & Unit Economics
- 4 to 5 core items engineered for rapid cross-utilization (e.g., potato/curd/bread base).
- Exactly 1 loss-leader anchor item priced under ₹20.
- Decoy pricing architecture (Target bundle vs. Deliberate premium anchor).
- Complete Unit Economics Table:
  | Item Name | Role / Category | Prep & Serve Time (s) | Raw Unit Cost (₹) | Selling Price (₹) | Gross Margin (₹ / %) | Projected Daily Vol |
  |---|---|---|---|---|---|---|
  | *Example: Bun Maska* | *Anchor / Loss-Leader* | *25s* | *₹11.50* | *₹18.00* | *₹6.50 (36.1%)* | *80 units* |

### Deliverable 3: Rush-Hour Workflow & Demand Engineering
- Sub-60-second fulfillment workflow for 15-minute class breaks.
- Token/QR/WhatsApp advance ordering protocol.
- Day-parting operational schedule:
  - Morning Rush (08:30 – 09:30)
  - Lunch Surge (12:30 – 14:00)
  - Evening Hangout (16:30 – 18:00)
- Demand modifiers: Rain impact, exam-week shift, Day 1–2 novelty decay mitigation.

### Deliverable 4: Waste Minimization & Zero-Waste Recipe Fallback
- FIFO storage and inventory rotation protocol.
- End-of-day clearance discounting rule (final 45 minutes).
- Pre-defined "Rescue Recipe" converting unsold cross-utilized stock into next-day revenue.

### Deliverable 5: 7-Day Financial Model & Reinvestment Mechanism
- Daily cash flow schedule from Day 1 through Day 7:
  | Day | Projected Revenue (₹) | Daily Inventory Restock (₹) | Operating Expense (₹) | Daily Net (₹) | Cumulative Cash Balance (₹) |
- Day-4 Reinvestment Protocol: How Day 1–3 cash surplus is recycled without breaching the 10% reserve.
- Scenario summary by Day 7: Conservative, Target, and Optimistic Net Profit.

### Deliverable 6: KPI Dashboard & Real-Time Action Triggers
- Core metrics: AOV, Counter Turnaround, Wastage %, Return on Working Capital.
- Threshold-action pairs:
  | KPI Metric | Target Benchmark | Breach Threshold | Mandatory Same-Day / Next-Day Action |
  |---|---|---|---|
  | Wastage % | < 5% | > 15% by Day 3 | Reduce next-day prep volume by 30% |
  | Average Order Value | > ₹35 | < ₹25 | Enforce combo decoy upselling script at register |

### Deliverable 7: Contingency & Failure-Mode Playbook
- Structured matrix handling 4 core failure scenarios:
  | Failure Trigger | Detection Point | Immediate Corrective Protocol | Cost / Margin Impact |
  |---|---|---|---|
  | Item Sell-Through Flop | Day 2 < 40% sold | Discontinue item, reallocate inventory to Rescue Recipe | Neutralizes spoilage loss |
  | Severe Weather / Footfall Shock | 2h into morning rush | Trigger reduced batch size, push WhatsApp pre-order combos | Protects margin |
  | Key Ingredient Price Spike | Supply purchase | Activate cross-chain substitute ingredient | Keeps COGS within ±5% |
  | Service Bottleneck > 90s | Break surge | Switch to pre-boxed single-SKU express queue | Restores throughput |

</deliverables_specification>

<output_formatting>
Generate the complete plan following Deliverables 1 through 7 sequentially under clean Markdown headers. All monetary amounts must be in Indian Rupees (₹). Ensure all calculations are mathematically coherent and fully derived from stated assumptions.
</output_formatting>
```
