# Product strategy accelerator

<https://www.reddit.com/r/promptingmagic/comments/1mua88x/this_is_the_ultimate_product_management_product/>

1. Executive Summary
2. Differentiation Strategies
3. Comprehensive Risk Register
4. Scenario Planning
5. 6-Month Roadmap
6. Revenue Models
7. Must-Have Features
8. Strategic Partnerships
9. User Personas
10. Product Names
11. Workshop Agenda
12. Value Propositions
13. Industry Trends
14. Solutions Sprint
15. Competitive Mapping
16. Innovation Backlog
17. Team Alignment Pack

## AI prompt

Step 1:  Copy and paste the following YAML block, filling in the details for your specific context. If a field is blank, the AI will infer from market norms.

```yaml
# --- Product Strategy Intake ---

# 1. Foundational Information
CompanyName: "[Insert Company Name]"
CompanyMissionVision: "[Briefly describe your company's core purpose and long-term vision]"
ProductName: "[Insert Product Name]"
ProductDescription: "[Provide a 1-2 paragraph description of the product, what it does, the core problem it solves, and its primary function.]"
CurrentBusinessGoals:
  - "[Objective 1, e.g., Increase market share by 15%]"
  - "[Objective 2, e.g., Achieve profitability]"
  - "[Objective 3, e.g., Expand into the European market]"

# 2. Market & Audience
TargetAudience: "[Describe your primary and secondary audience segments. e.g., 'Marketing Managers at mid-size tech companies']"
SpecificUserProblem: "[Clearly define the primary pain point or challenge your product solves for your users.]"

# 3. Competitive Landscape
DirectCompetitors:
  - "[Competitor 1]"
  - "[Competitor 2]"
  - "[Competitor 3]"
IndirectCompetitors:
  - "[Indirect Competitor 1]"
  - "[Indirect Competitor 2]"

# 4. Product Details & Vision
CurrentProductStage: "[Pre-launch/Growth/Maturity]"
KeyFeaturesUnderConsideration:
  - "[Feature A]"
  - "[Feature B]"
LongTermProductVision: "[Where do you see this product in the next 3-5 years? What is its ultimate potential?]"

# 5. Technical & Platform Context
TechnicalDebt: "[Low/Medium/High]"
PlatformCapabilities: "[API-first/Monolithic/Microservices]"
DataMaturity: "[Basic/Intermediate/Advanced]"
AIReadiness: "[None/Exploring/Implementing/Advanced]"

# 6. Market Dynamics
MarketCategory: "[Creating new/Disrupting existing/Competing in established]"
NetworkEffects: "[None/Weak/Strong/Critical]"
RegulatoryConstraints: "[List key regulations affecting product, e.g., GDPR, HIPAA]"

# 7. Output Controls (Optional)
OUTPUT_FORMATS: ["markdown", "json", "mermaid", "csv"] # Specify desired output formats
```

Step 2: Use your completed YAML block from step 1 above. Copy/paste it into your AI, and copy/paste the prompt below, then enter.

Prompt:

```prompt
Act as a world-class Chief Product Officer and strategic advisor. Using the detailed information provided in the YAML Intake below, generate a comprehensive and actionable product strategy document.

Strictly adhere to the following operating rules, methods, and deliverable structure.

## Operating Rules

- **Assumptions:** Label every assumption and confidence level (High/Med/Low).

- **Recommendations:** For every recommendation include: Why now, Expected impact, Leading indicators, Effort class (S/M/L), Risk flags.

- **Conciseness:** Prefer concise tables. Put the “so what” first.

- **Prioritization:** Use RICE and WSJF in parallel; show both, then reconcile with reasoning.

  - RICE = Reach × Impact × Confidence ÷ Effort (1–10 scales; Effort in person-weeks).

  - WSJF = Cost of Delay ÷ Job Size; Cost of Delay = (User/Revenue/Time criticality).

- **Risk Scoring:** Risk score = Likelihood (1–5) × Impact (1–5). Include Owner, Trigger, Mitigation, Fallback.

- **Roadmap:** Show milestones by month, dependencies, and entry/exit criteria (“definition of done”).

- **Personas:** Use JTBD format and buying committee roles where B2B (Economic, Technical, User, Champion).

- **Legal:** Keep names/claims legally cautious; note where trademark/domain checks are needed.

## Dynamic Adaptation Rules

Based on the `CurrentProductStage`, automatically adjust emphasis:

- If Pre-launch: Focus heavily on MVP definition, early adopter feedback loops, learning velocity, and validating core assumptions (Deliverables 7, 9, 14).

- If Growth: Emphasize scaling systems, feature velocity, market expansion, and competitive differentiation (Deliverables 2, 5, 8, 15).

- If Maturity: Prioritize retention strategies, efficiency, platform plays, and exploring new revenue models to combat commoditization (Deliverables 6, 13, 16, 17).

Deliverables (in this exact order)

1. Executive Summary (1 page)
2. Differentiation Strategies (10)
3. Comprehensive Risk Register (12)
4. Future Scenario Planning (3-4 scenarios)
5. 6-Month Product Roadmap
6. Alternative Revenue Models (5)
7. Must-Have Features (10)
8. Strategic Partnerships (10)
9. User Personas (5)
10. Product Names (20) with Rationale
11. Structured 2-Hour Workshop Agenda
12. Targeted Value Propositions (7)
13. Emerging Industry Trends (10)
14. Solutions Sprint: 10 Ideas for a Defined Challenge
15. Competitive Landscape Mapping (up to 10 competitors)
16. Bold Innovation Backlog (15)
17. Team Alignment Pack

Output Artifacts (Mermaid Diagrams & CSV Extracts)
