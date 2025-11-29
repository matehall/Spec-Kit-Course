# Module 4 Review Quiz

**Module:** 4 - Advanced Techniques  
**Quiz:** Module 4 Assessment  
**Date:** November 29, 2025  
**Time:** 25-35 minutes  
**Passing Score:** 80% (16/20 questions)

---

## 📋 Instructions

This quiz tests your understanding of advanced Spec Kit techniques:
- Clarifying underspecified requirements
- Cross-artifact validation and analysis
- Quality assurance through checklists
- Integrating advanced commands into workflow

---

## Section 1: Clarification (5 questions)

### Question 1
**When should you use `/clarify`?**

- [ ] A. Only when explicitly asked by stakeholders
- [ ] B. When you encounter vague, ambiguous, or missing details
- [ ] C. After implementation is complete
- [ ] D. Never – just make your best guess

<details>
<summary>Answer</summary>

**B. When you encounter vague, ambiguous, or missing details**

Use `/clarify` proactively when:
- Requirements are vague ("make it user-friendly")
- Edge cases aren't specified
- Technical details are missing
- Conflicts exist between documents
</details>

---

### Question 2
**A specification says "search should be fast." How should you clarify this?**

- [ ] A. Leave it as is – everyone knows what "fast" means
- [ ] B. Define specific, measurable performance targets (e.g., < 500ms p95)
- [ ] C. Ask the stakeholder what they mean
- [ ] D. Implement and see if anyone complains

<details>
<summary>Answer</summary>

**B. Define specific, measurable performance targets**

Convert subjective terms into objective, measurable criteria:
- "Fast" → < 500ms response time (p95)
- "User-friendly" → Specific UX requirements
- "Secure" → Specific security standards

Document these clarifications in the specification.
</details>

---

### Question 3
**You've clarified a requirement in the spec. What else should you update?**

- [ ] A. Nothing – just the spec
- [ ] B. The plan and tasks if they're affected
- [ ] C. Only the code
- [ ] D. The constitution

<details>
<summary>Answer</summary>

**B. The plan and tasks if they're affected**

Maintain consistency across all artifacts:
1. Update specification (the requirement)
2. Update plan (if technical approach changes)
3. Update tasks (if work breakdown changes)
4. Update tests (if acceptance criteria change)

All documents must remain aligned.
</details>

---

### Question 4
**Which is a good clarification?**

- [ ] A. "Make it work properly"
- [ ] B. "Handle errors"
- [ ] C. "Email validation must reject invalid formats using RFC 5322 regex, with user-friendly error message: 'Please enter a valid email address'"
- [ ] D. "Do it the standard way"

<details>
<summary>Answer</summary>

**C. Specific, detailed clarification with concrete criteria**

Good clarifications are:
- **Specific** (RFC 5322 regex)
- **Actionable** (reject invalid formats)
- **Complete** (includes error message)
- **Unambiguous** (no guessing needed)

A, B, and D are still vague.
</details>

---

### Question 5
**You're clarifying "authentication requirements." What method should you use?**

- [ ] A. Just ask "What do you want?"
- [ ] B. Apply the 5W1H method (Who, What, When, Where, Why, How)
- [ ] C. Copy from another project
- [ ] D. Implement and iterate

<details>
<summary>Answer</summary>

**B. Apply the 5W1H method**

Example:
- **Who:** All users, or just certain roles?
- **What:** Email/password, social login, or both?
- **When:** Session duration? Remember me?
- **Where:** Web app, mobile app, or both?
- **Why:** Security requirements? Compliance needs?
- **How:** JWT, OAuth2, session cookies?

Systematic questioning ensures thorough clarification.
</details>

---

## Section 2: Analysis (5 questions)

### Question 6
**What is "vertical consistency"?**

- [ ] A. Code formatted with proper indentation
- [ ] B. Alignment from requirements (spec) → plan → tasks → code
- [ ] C. All features in one vertical
- [ ] D. Consistency within a single file

<details>
<summary>Answer</summary>

**B. Alignment from requirements (spec) → plan → tasks → code**

Vertical consistency ensures:
- Every requirement has a plan
- Every plan component has tasks
- Every task has implementation
- No orphaned or missing items
</details>

---

### Question 7
**During `/analyze`, you find code implements features not in the spec. This is:**

- [ ] A. Great – more features!
- [ ] B. Scope creep – needs to be documented or removed
- [ ] C. No problem as long as it works
- [ ] D. Update the spec to match the code

<details>
<summary>Answer</summary>

**B. Scope creep – needs to be documented or removed**

Unspecified features are problematic:
- Not properly tested
- No acceptance criteria
- May not meet actual needs
- Creates maintenance burden

**Action:** Either create proper specs for them or remove them to stay focused.
</details>

---

### Question 8
**The plan says "use Repository pattern" but code uses direct database queries. What should you do?**

- [ ] A. Ignore it – code works
- [ ] B. Update plan to match code
- [ ] C. Refactor code to follow plan (if pattern is right) or update plan with justification
- [ ] D. Create a new feature branch

<details>
<summary>Answer</summary>

**C. Refactor code to follow plan (if pattern is right) or update plan with justification**

**Option 1:** Plan is correct → Refactor code to use Repository pattern
**Option 2:** Direct queries are better → Update plan and document why

Never leave documentation and code inconsistent!
</details>

---

### Question 9
**Which should trigger cross-artifact analysis?**

- [ ] A. After every line of code
- [ ] B. At major milestones (spec complete, plan complete, before review)
- [ ] C. Only if you suspect problems
- [ ] D. Never – trust that everything is aligned

<details>
<summary>Answer</summary>

**B. At major milestones**

Run `/analyze`:
- After completing specification
- After completing plan
- After major implementation chunks
- Before code review
- Before deployment

Balance thoroughness with productivity.
</details>

---

### Question 10
**What is "horizontal consistency"?**

- [ ] A. Code aligned horizontally on screen
- [ ] B. Consistency across similar features (e.g., all auth endpoints follow same patterns)
- [ ] C. Features laid out horizontally in project
- [ ] D. Cross-team consistency

<details>
<summary>Answer</summary>

**B. Consistency across similar features**

Horizontal consistency means:
- Similar features use similar patterns
- Naming conventions are consistent
- Error handling approaches are uniform
- Architectural decisions are aligned

Example: All API endpoints follow same structure, error format, authentication approach.
</details>

---

## Section 3: Checklists (5 questions)

### Question 11
**What makes a good checklist item?**

- [ ] A. Subjective and open to interpretation
- [ ] B. Binary (clear pass/fail) and objective
- [ ] C. As detailed as possible, spanning multiple pages
- [ ] D. Covering multiple concerns in one item

<details>
<summary>Answer</summary>

**B. Binary (clear pass/fail) and objective**

Good checklist items:
- ✓ "All functions have names" (objective)
- ✓ "API response time < 200ms p95" (measurable)
- ✗ "Code is good quality" (subjective)
- ✗ "Performance is acceptable" (ambiguous)
</details>

---

### Question 12
**How long should a checklist be?**

- [ ] A. 1-5 items (too short is better than too long)
- [ ] B. 15-25 items ideally (one screenful)
- [ ] C. 100+ items (more comprehensive is better)
- [ ] D. Exactly 10 items always

<details>
<summary>Answer</summary>

**B. 15-25 items ideally**

**Why:**
- One screenful – no scrolling fatigue
- Focused on essentials
- Actually gets used (not overwhelming)

If you need more:
- Split into multiple checklists (by phase)
- Or tier them (Critical / Important / Nice-to-have)
</details>

---

### Question 13
**A bug slipped through your checklist. What should you do?**

- [ ] A. Abandon checklists – they don't work
- [ ] B. Blame the checklist
- [ ] C. Update the checklist to catch this type of bug in future
- [ ] D. Keep using the same checklist

<details>
<summary>Answer</summary>

**C. Update the checklist to catch this type of bug in future**

Checklists are **living documents**:

1. Analyze why bug wasn't caught
2. Add item to prevent it
3. Share learning with team
4. Checklist improves over time

Example:
```markdown
Bug: User could submit empty email

Checklist addition:
- [ ] All required fields validated on both client and server
- [ ] Empty string inputs explicitly rejected
- [ ] Tests include empty string edge cases
```
</details>

---

### Question 14
**When should you use a checklist?**

- [ ] A. Only before deployment
- [ ] B. At key quality gates (after spec, plan, implementation, review)
- [ ] C. Only for complex features
- [ ] D. Never – they slow you down

<details>
<summary>Answer</summary>

**B. At key quality gates**

Use checklists:
- ✓ After specification (completeness check)
- ✓ After plan (architecture validation)
- ✓ After implementation (code quality)
- ✓ Before review (comprehensive check)
- ✓ Before deployment (production readiness)

Scale rigor to change size (full checklist for features, lighter for small bugs).
</details>

---

### Question 15
**Your checklist has both "critical" and "nice-to-have" items. How should you structure it?**

- [ ] A. Mix them together randomly
- [ ] B. Create tiers: Critical (must check) / Important (should check) / Optional (could check)
- [ ] C. Only include critical items
- [ ] D. Only include nice-to-have items

<details>
<summary>Answer</summary>

**B. Create tiers**

**Example:**
```markdown
## Critical (Must Pass - 8 items)
- Security checks
- Data integrity
- Core functionality

## Important (Should Pass - 12 items)
- Error handling
- Edge cases
- Test coverage

## Nice-to-Have (Optional - 5 items)
- Code style polish
- Documentation extras
- Optimizations
```

This allows prioritization when time is limited.
</details>

---

## Section 4: Integration (5 questions)

### Question 16
**What is a "quality gate"?**

- [ ] A. A physical gate at the office
- [ ] B. A checkpoint where work must pass quality criteria before proceeding
- [ ] C. A senior developer who approves all work
- [ ] D. A tool for measuring code quality

<details>
<summary>Answer</summary>

**B. A checkpoint where work must pass quality criteria before proceeding**

Example workflow:
```
Spec → [Quality Gate 1] → Plan → [Quality Gate 2] → Implement
```

At each gate:
- Run checklist
- Run analysis
- Fix issues
- Only proceed when criteria met

Prevents compounding errors.
</details>

---

### Question 17
**You're fixing a typo in a comment. Which advanced commands should you use?**

- [ ] A. Full workflow: /specify, /plan, /tasks, /checklist, /analyze
- [ ] B. None – just fix it
- [ ] C. Only /analyze
- [ ] D. Only /checklist

<details>
<summary>Answer</summary>

**B. None – just fix it**

**Scale your process:**
- Typo fix: Just do it
- Small bug: Light process
- Enhancement: Moderate process
- New feature: Full process

Don't over-process trivial changes!
</details>

---

### Question 18
**The best workflow integration approach is:**

- [ ] A. Use all commands for every change, no matter how small
- [ ] B. Never use advanced commands – they slow you down
- [ ] C. Scale rigor to change size and risk
- [ ] D. Only use commands when someone is watching

<details>
<summary>Answer</summary>

**C. Scale rigor to change size and risk**

**Decision factors:**
- Change size (1 line vs 1000 lines)
- Risk (typo vs payment processing)
- Ambiguity (clear vs unclear requirements)
- Impact (internal tool vs user-facing)

**More risk/size/ambiguity → More rigor**
</details>

---

### Question 19
**During implementation, `/analyze` finds a spec-plan conflict. You should:**

- [ ] A. Ignore it – you're almost done
- [ ] B. Stop, resolve conflict, update artifacts, then continue
- [ ] C. Note it in a TODO comment and continue
- [ ] D. Finish feature first, then maybe fix it

<details>
<summary>Answer</summary>

**B. Stop, resolve conflict, update artifacts, then continue**

**Why:**
1. Conflicts compound over time
2. Context is fresh now
3. Easier to fix before building on top
4. Maintains documentation trust

**Process:**
1. Stop work (commit current state)
2. Analyze conflict
3. Clarify correct approach
4. Update all affected artifacts
5. Resume implementation
</details>

---

### Question 20
**The purpose of integrating clarify/analyze/checklist is to:**

- [ ] A. Make development slower and more bureaucratic
- [ ] B. Catch errors early, maintain quality, and reduce rework
- [ ] C. Justify higher billing rates
- [ ] D. Impress stakeholders with process

<details>
<summary>Answer</summary>

**B. Catch errors early, maintain quality, and reduce rework**

**Benefits:**
- Find issues when they're cheap to fix
- Maintain documentation accuracy
- Reduce debugging time
- Build with confidence
- Enable fearless refactoring

**Paradox:** Going slower (with checks) makes you go faster (fewer bugs, less rework).
</details>

---

## 🎯 Quiz Complete!

### Scoring

**Count your correct answers:**

- **18-20 (90-100%):** 🌟 **Excellent!** You've mastered advanced techniques
- **16-17 (80-89%):** ✅ **Pass!** You understand the concepts well
- **13-15 (65-79%):** ⚠️ **Review Needed** – Revisit weak areas
- **< 13 (< 65%):** 📚 **More Study Needed** – Re-read Module 4 lessons

### Your Score: ____ / 20 (____%)

---

## 📊 Section Breakdown

- **Section 1 (Clarification):** ____ / 5
- **Section 2 (Analysis):** ____ / 5
- **Section 3 (Checklists):** ____ / 5
- **Section 4 (Integration):** ____ / 5

---

## 🎓 Key Takeaways

**If you passed:**

You now understand:
- ✓ How to clarify ambiguous requirements systematically
- ✓ How to validate consistency across artifacts
- ✓ How to use checklists for quality assurance
- ✓ How to integrate advanced commands into your workflow
- ✓ How to scale process rigor appropriately

**If you need review:**

Focus on sections where you scored < 4/5, then retake the quiz.

---

## ✅ What's Next?

**Module 5: Development Phases** awaits!

You'll learn how to apply Spec-Driven Development to:
- Greenfield (0-to-1) projects
- Creative exploration and prototyping
- Brownfield (iterative enhancement) projects

Different phases require different approaches – let's master them all!

---

*Back to: [Lesson 16: Advanced Workflow Integration](./Lesson-16-Advanced-Workflow-Integration.md)*  
*Next: Module 5 - [Lesson 17: 0-to-1 Development (Greenfield)](../Module-05-Development-Phases/Lesson-17-0-to-1-Development-Greenfield.md)*
