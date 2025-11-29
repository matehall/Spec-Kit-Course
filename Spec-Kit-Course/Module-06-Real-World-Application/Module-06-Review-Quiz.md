# Module 6 Review Quiz: Real-World Application

**Module 6: Real-World Application**  
**Date:** November 29, 2025  
**Questions:** 20

---

## Instructions

This quiz covers Lessons 20-22, focusing on enterprise considerations, technology independence, and troubleshooting. Answer all questions, then check your answers at the end.

**Passing Score:** 16/20 (80%)

---

## Questions

### Enterprise Considerations (Lessons 20)

**1. What is the primary purpose of a Spec Kit governance board in an enterprise?**

A) To write all specifications for the company  
B) To establish standards, resolve disputes, and ensure consistency  
C) To replace individual team decision-making  
D) To audit every specification before implementation  

---

**2. In a distributed team, what is the MOST critical factor for successful Spec Kit adoption?**

A) Everyone must use the same IDE  
B) All developers must be in the same time zone  
C) Clear communication protocols and asynchronous-friendly workflows  
D) Having a dedicated Spec Kit administrator  

---

**3. Which compliance consideration is MOST important when using AI agents with specifications?**

A) The AI model's training data sources  
B) Ensuring sensitive information isn't leaked to AI providers  
C) The AI's ability to write perfect code  
D) The AI's understanding of business logic  

---

**4. What does "progressive adoption" mean in the context of enterprise Spec Kit rollout?**

A) Using increasingly complex specifications over time  
B) Starting with pilot teams and expanding based on success  
C) Gradually teaching developers to write better  
D) Implementing features in progressive order  

---

**5. In a legacy codebase migration, what should you do FIRST?**

A) Rewrite everything with specifications  
B) Map critical paths and high-change areas for initial spec coverage  
C) Delete all old code  
D) Stop all new development  

---

### Technology Independence (Lesson 21)

**6. What makes Spec Kit "technology independent"?**

A) It's written in multiple programming languages  
B) It focuses on WHAT to build, not HOW (language/framework)  
C) It works with any AI agent  
D) It doesn't require Git  

---

**7. In a polyglot architecture with Python, Go, and JavaScript services, how should shared business logic be specified?**

A) Write separate specs for each language  
B) Choose the "primary" language and write specs for that  
C) Write language-agnostic specs focused on behavior and contracts  
D) Don't specify shared logic, let each team decide  

---

**8. When migrating from React to Svelte, what should happen to your specifications?**

A) Rewrite all specs for Svelte  
B) Core behavior specs remain valid; update implementation-specific plans  
C) Archive old specs and start fresh  
D) Keep React specs and create parallel Svelte specs  

---

**9. What is a "contract specification"?**

A) Legal agreements between teams  
B) Interface definitions that specify inputs, outputs, and behavior without implementation  
C) Employment contracts for developers  
D) Service-level agreements  

---

**10. Which specification element is MOST likely to be framework-agnostic?**

A) Component lifecycle methods  
B) State management approach  
C) Business rule validation logic  
D) Routing configuration  

---

### Troubleshooting & Debugging (Lesson 22)

**11. What is the OBSERVE framework in debugging?**

A) A way to watch code execution  
B) A systematic approach: Observe, Backtrack, Simplify, Experiment, Record, Verify, Extract lesson  
C) A Git command for tracking changes  
D) An AI agent instruction protocol  

---

**12. When you encounter merge conflicts in spec files, what should you do FIRST?**

A) Always choose "ours"  
B) Delete both versions and start over  
C) Understand the context and intentions behind both changes  
D) Ask your manager to decide  

---

**13. What is "spec drift"?**

A) Specifications moving to different folders  
B) Git branch divergence  
C) Specifications becoming outdated as code evolves  
D) Team members disagreeing on spec format  

---

**14. An AI agent consistently generates incorrect code from a spec that seems clear. What's a likely cause?**

A) The AI is broken  
B) The spec contains ambiguous language, conflicting requirements, or insufficient context  
C) The AI doesn't like your writing style  
D) The spec is too short  

---

**15. What is the danger of "quick fix" debugging?**

A) It's too fast to be thorough  
B) It addresses symptoms rather than root causes, creating technical debt  
C) It makes team members look bad  
D) It requires too much documentation  

---

**16. When should you use `spec-kit analyze`?**

A) Only when something breaks  
B) Only before major releases  
C) Regularly (e.g., weekly) to catch issues early  
D) Never, it's too slow  

---

**17. What is a circular dependency in specifications?**

A) Using circle diagrams instead of squares  
B) When Spec A requires Spec B, which requires Spec C, which requires Spec A  
C) When specs reference each other at all  
D) When specs are organized in folders  

---

**18. What should a pre-commit hook do in a Spec Kit workflow?**

A) Prevent all commits  
B) Validate specs and check for spec-code alignment before allowing commit  
C) Automatically fix all issues  
D) Send emails to the team  

---

### Integrated Scenarios

**19. Your enterprise is adopting Spec Kit, but developers complain the workflow is too slow. What should you do?**

A) Force compliance through policy  
B) Abandon Spec Kit  
C) Investigate specific pain points and automate tedious steps  
D) Hire more developers  

---

**20. You're migrating a monolithic PHP application to microservices (Go, Python, Node.js). How should you handle specifications?**

A) Keep PHP-specific specs and create new specs for each microservice language  
B) Write language-agnostic behavior specs, then create implementation plans for each service  
C) Don't use specs during migration (too complex)  
D) Wait until migration is complete to add specs  

---

## Answer Key

<details>
<summary><strong>Click to Reveal Answers</strong></summary>

1. **B** - Governance boards establish standards and ensure consistency
2. **C** - Clear communication and async-friendly workflows are critical for distributed teams
3. **B** - Preventing sensitive data leakage to AI providers is paramount
4. **B** - Progressive adoption means starting with pilots and expanding
5. **B** - Map critical paths first for focused, high-value spec coverage
6. **B** - Technology independence focuses on WHAT, not HOW
7. **C** - Write language-agnostic specs focused on behavior
8. **B** - Core behavior specs remain valid; update implementation details
9. **B** - Contract specs define interfaces without implementation
10. **C** - Business rules are framework-agnostic
11. **B** - OBSERVE is a systematic debugging framework
12. **C** - Understand context and intentions first
13. **C** - Spec drift is specifications becoming outdated
14. **B** - Likely causes are ambiguity, conflicts, or insufficient context
15. **B** - Quick fixes address symptoms, not root causes
16. **C** - Regular use catches issues early
17. **B** - Circular dependency: A→B→C→A
18. **B** - Pre-commit hooks should validate specs and alignment
19. **C** - Investigate pain points and automate
20. **B** - Write behavior specs, then implementation plans per service

</details>

---

## Scoring Guide

**18-20 correct:** Excellent! You've mastered real-world application concepts.  
**16-17 correct:** Good understanding. Review any missed questions.  
**14-15 correct:** Passing. Consider reviewing the lessons for deeper understanding.  
**Below 14:** Review Module 6 lessons and retake the quiz.

---

## Detailed Explanations

<details>
<summary><strong>Question 1 Explanation</strong></summary>

**Correct Answer: B**

A governance board doesn't write specs or replace team autonomy. Its role is to:
- Establish organization-wide standards
- Resolve cross-team specification disputes
- Ensure consistency across departments
- Provide guidance and best practices
- Facilitate knowledge sharing

This enables teams to work independently while maintaining coherence.
</details>

<details>
<summary><strong>Question 3 Explanation</strong></summary>

**Correct Answer: B**

Compliance risk primarily involves:
- **Data privacy:** Sending specs containing PII, passwords, or proprietary algorithms to external AI services
- **Intellectual property:** Leaking trade secrets or patented processes
- **Regulatory compliance:** GDPR, HIPAA, SOC 2 requirements

Solutions include:
- Using self-hosted AI models
- Sanitizing specs before sending to external AIs
- Clear policies on what can be shared
- Audit trails of AI interactions
</details>

<details>
<summary><strong>Question 7 Explanation</strong></summary>

**Correct Answer: C**

In polyglot architectures, specifications should focus on:
- **Behavior:** What the system does
- **Contracts:** Input/output interfaces
- **Business rules:** Language-independent logic

Example:
```markdown
## User Balance Calculation (REQ-BAL-001)

**Inputs:**
- user_id: string (UUID v4)
- currency: string (ISO 4217 code)

**Outputs:**
- available_balance: decimal (2 decimal places)
- pending_transactions: array of transaction objects

**Business Rules:**
1. Available balance = ledger balance - pending debits
2. Include transactions from last 90 days only
3. Convert all amounts to requested currency using daily rate

**Success Criteria:**
- Calculation completes in <100ms
- Results match across all service implementations
- Audit trail captures calculation details
```

Each service implements this differently, but the behavior is identical.
</details>

<details>
<summary><strong>Question 11 Explanation</strong></summary>

**Correct Answer: B**

The OBSERVE framework provides systematic debugging:

- **O**bserve symptoms carefully
- **B**acktrack to last known good state
- **S**implify and isolate the problem
- **E**xperiment with minimal changes
- **R**ecord results and observations
- **V**erify the fix works
- **E**xtract lessons for prevention

This prevents random "try things until something works" debugging.
</details>

<details>
<summary><strong>Question 14 Explanation</strong></summary>

**Correct Answer: B**

Common causes of AI confusion:
1. **Ambiguous language:** "The system should be fast" (how fast?)
2. **Conflicting requirements:** "Must support 1M users" + "SQLite database"
3. **Insufficient context:** Missing dependencies, architecture constraints
4. **Hidden assumptions:** Expecting the AI to know your tech stack
5. **Spec too long:** Exceeds AI context window

Solution: Run `spec-kit clarify` to identify underspecified areas, then refine.
</details>

<details>
<summary><strong>Question 17 Explanation</strong></summary>

**Correct Answer: B**

Circular dependencies create impossible implementation orders:
```
REQ-001 (Dashboard) depends on REQ-003 (Auth)
REQ-002 (Admin) depends on REQ-001 (Dashboard)
REQ-003 (Auth) depends on REQ-002 (Admin for user mgmt)
```

**Detection:** `spec-kit analyze --check-dependencies`

**Resolution:** Extract shared foundation layer that has no dependencies.
</details>

<details>
<summary><strong>Question 20 Explanation</strong></summary>

**Correct Answer: B**

Migration strategy:
1. **Write behavior specs** for monolith's functionality (technology-independent)
2. **Decompose by domain** (users, orders, payments, etc.)
3. **Create implementation plans** for each microservice in its target language
4. **Validate equivalence** between monolith and microservices using same specs

The behavior specs serve as:
- Migration checklist
- Regression test scenarios
- Documentation of system behavior
- Contract between old and new systems

This ensures you don't lose functionality during migration.
</details>

---

## Common Mistakes to Avoid

### Enterprise Adoption
❌ Forcing top-down adoption without pilot success  
✅ Demonstrate value with pilot teams, then expand organically

❌ Creating rigid, one-size-fits-all processes  
✅ Establish principles, let teams adapt to their context

### Technology Independence
❌ Including framework-specific details in specs  
✅ Focus on behavior, defer implementation to plans

❌ Rewriting specs for every technology change  
✅ Write once, implement many times

### Troubleshooting
❌ Jumping to solutions without diagnosis  
✅ Use systematic debugging frameworks

❌ Applying quick fixes without understanding root causes  
✅ Invest time in proper fixes and prevention

---

## Reflection Questions

After completing this quiz, consider:

1. **What surprised you most about enterprise considerations?**
   - How does your organization compare?
   - What changes could improve adoption?

2. **How technology-independent are your current specs?**
   - Can you swap frameworks without rewriting specs?
   - What would you need to change?

3. **What's your debugging process?**
   - Do you follow a systematic approach?
   - How could you improve?

---

## Next Steps

Ready for Module 7: Mastery? The final module covers:
- User-centric development
- Iterative and creative processes
- The future of spec-driven development
- Your journey forward

Continue building your expertise!

---

## Navigation

← [Previous: Lesson 22 - Troubleshooting & Debugging](Lesson-22-Troubleshooting-and-Debugging.md)  
→ [Next: Module 7 - Mastery](../Module-07-Mastery/)  
↑ [Back to Module 6](../Module-06-Real-World-Application/)  
🏠 [Course Home](../00-Course-Overview.md)
