# Module 5 Review Quiz

**Module:** 5 - Development Phases  
**Quiz:** Module 5 Assessment  
**Date:** November 29, 2025  
**Time:** 20-30 minutes  
**Passing Score:** 80% (12/15 questions)

---

## Section 1: Greenfield Development (5 questions)

### Question 1
**What is the main advantage of greenfield development?**

- [ ] A. It's faster than brownfield
- [ ] B. No legacy constraints, can choose optimal architecture
- [ ] C. No need for planning
- [ ] D. Guaranteed success

<details>
<summary>Answer</summary>

**B. No legacy constraints, can choose optimal architecture**

Greenfield gives you freedom to choose modern technologies, design optimal architecture, and establish best practices from day one.
</details>

---

### Question 2
**In greenfield development, should you build all planned features in the first release?**

- [ ] A. Yes, ship everything at once
- [ ] B. No, start with MVP (minimum viable product)
- [ ] C. Build half the features
- [ ] D. Only build if time permits

<details>
<summary>Answer</summary>

**B. No, start with MVP**

Focus on core value proposition. Ship minimum set of features that deliver value, then iterate based on real user feedback.
</details>

---

### Question 3
**What does "building vertical slices" mean?**

- [ ] A. Building all database models first, then all APIs, then all UI
- [ ] B. Building complete features (DB → API → UI) one at a time
- [ ] C. Building the backend before frontend
- [ ] D. Building features in alphabetical order

<details>
<summary>Answer</summary>

**B. Building complete features (DB → API → UI) one at a time**

Each slice is a complete, working feature across all layers. Benefits: see progress early, test integration continuously, deliver value incrementally.
</details>

---

### Question 4
**You're 6 weeks into greenfield development and realize your architecture choice was wrong. What should you do?**

- [ ] A. Continue anyway (sunk cost)
- [ ] B. Evaluate cost of changing vs continuing, then decide
- [ ] C. Start completely over
- [ ] D. Ignore it and hope it works out

<details>
<summary>Answer</summary>

**B. Evaluate cost of changing vs continuing, then decide**

Greenfield is the best time to change. Don't fall for sunk cost fallacy. If architecture is fundamentally wrong and will cause ongoing pain, fix it now rather than accumulating years of technical debt.
</details>

---

### Question 5
**What should a greenfield constitution include?**

- [ ] A. Specific feature requirements
- [ ] B. Project-wide standards (tech stack, architecture patterns, code style)
- [ ] C. User stories
- [ ] D. Task assignments

<details>
<summary>Answer</summary>

**B. Project-wide standards**

Constitution defines HOW you build (standards, patterns, conventions), not WHAT you build (features). It's the foundation that all features follow.
</details>

---

## Section 2: Creative Exploration (5 questions)

### Question 6
**When should you use creative exploration instead of formal specification?**

- [ ] A. Always – specs are outdated
- [ ] B. Never – always write specs first
- [ ] C. When requirements are genuinely unclear and need discovery
- [ ] D. Only for side projects

<details>
<summary>Answer</summary>

**C. When requirements are genuinely unclear and need discovery**

Use exploration when innovation is needed, user needs must be discovered, or you're testing multiple approaches. Use formal specs when requirements are clear.
</details>

---

### Question 7
**How long should creative exploration be time-boxed?**

- [ ] A. No time limit – explore until perfect
- [ ] B. 1-3 weeks typically
- [ ] C. 1 day maximum
- [ ] D. 6 months minimum

<details>
<summary>Answer</summary>

**B. 1-3 weeks typically**

Set a deadline and stick to it. After exploration, make a decision: build it, pivot, or kill it. Don't let exploration become endless.
</details>

---

### Question 8
**After exploration, you find one feature works great, two are mediocre. What should you do?**

- [ ] A. Build all three (we explored them all)
- [ ] B. Build only the winner
- [ ] C. Build none (need all three to be great)
- [ ] D. Explore for another month

<details>
<summary>Answer</summary>

**B. Build only the winner**

Ship one amazing feature, not three mediocre ones. Kill your darlings – just because you built a prototype doesn't mean you should ship it.
</details>

---

### Question 9
**Should prototype code be refactored for production or rewritten?**

- [ ] A. Always refactor (don't waste the code)
- [ ] B. Usually rewrite, salvaging learnings and key algorithms
- [ ] C. Always rewrite from scratch
- [ ] D. Ship prototype code as-is

<details>
<summary>Answer</summary>

**B. Usually rewrite, salvaging learnings and key algorithms**

Prototypes are for learning, not shipping. Extract what you learned, salvage any solid algorithms, but rewrite with proper architecture, tests, and error handling.
</details>

---

### Question 10
**What should you track during creative exploration?**

- [ ] A. Nothing – just build
- [ ] B. Everything: user interactions, engagement, success rates, feedback
- [ ] C. Only revenue
- [ ] D. Only code quality

<details>
<summary>Answer</summary>

**B. Everything: user interactions, engagement, success rates, feedback**

Heavy instrumentation is critical. Track what users actually do (not what they say). Data drives decisions about what to build.
</details>

---

## Section 3: Brownfield Development (5 questions)

### Question 11
**What's the golden rule of brownfield development?**

- [ ] A. Move fast and break things
- [ ] B. Never break existing functionality
- [ ] C. Rewrite everything from scratch
- [ ] D. Avoid making any changes

<details>
<summary>Answer</summary>

**B. Never break existing functionality**

Existing system serves real users. Your enhancements must not disrupt them. Use incremental changes, feature flags, and backward compatibility.
</details>

---

### Question 12
**How should you handle breaking database schema changes?**

- [ ] A. Deploy change and update code simultaneously
- [ ] B. Use multi-phase deployment (add new, dual-write, switch reads, remove old)
- [ ] C. Schedule downtime and do it all at once
- [ ] D. Avoid database changes entirely

<details>
<summary>Answer</summary>

**B. Use multi-phase deployment**

Phase 1: Add new column (old code still works)
Phase 2: Dual-write (write to both)
Phase 3: Switch reads (use new column)
Phase 4: Remove old column (weeks later)

Zero downtime, backward compatible, can rollback at any step.
</details>

---

### Question 13
**What's the purpose of feature flags in brownfield development?**

- [ ] A. Just to make code more complex
- [ ] B. Gradual rollout, kill switch, A/B testing, beta features
- [ ] C. Only for testing environments
- [ ] D. Marketing purposes

<details>
<summary>Answer</summary>

**B. Gradual rollout, kill switch, A/B testing, beta features**

Feature flags enable:
- Roll out to 1% → 10% → 100% safely
- Instant kill switch if issues found
- Test new vs old approaches
- Give beta users early access
</details>

---

### Question 14
**You find ugly legacy code. Should you refactor it while adding your feature?**

- [ ] A. Always refactor bad code
- [ ] B. Only if it affects your feature or blocks you
- [ ] C. Never touch working code
- [ ] D. Rewrite the entire module

<details>
<summary>Answer</summary>

**B. Only if it affects your feature or blocks you**

If old code works and isn't touched by your feature, leave it alone (don't introduce risk). If it blocks you or must change, refactor carefully with tests. Keep refactoring separate from feature work.
</details>

---

### Question 15
**What's the best approach to brownfield enhancements?**

- [ ] A. Big rewrites (clean slate)
- [ ] B. Incremental changes with gradual rollout
- [ ] C. Change everything at once
- [ ] D. Avoid enhancements (too risky)

<details>
<summary>Answer</summary>

**B. Incremental changes with gradual rollout**

Small changes = smaller blast radius. Gradual rollout = catch issues early with small user subset. Can pause or rollback at any point. Safer than big-bang releases.
</details>

---

## 🎯 Quiz Complete!

### Your Score: ____ / 15 (____%)

**18-20 (90-100%):** 🌟 Excellent mastery!  
**16-17 (80-89%):** ✅ Pass – good understanding  
**13-15 (65-79%):** ⚠️ Review recommended  
**< 13 (< 65%):** 📚 Re-read Module 5

---

## 📊 Section Breakdown

- **Greenfield:** ____ / 5
- **Exploration:** ____ / 5
- **Brownfield:** ____ / 5

---

## ✅ What's Next?

**Module 6: Real-World Application** covers:
- Enterprise considerations
- Technology independence
- Troubleshooting & debugging

Ready to learn how Spec-Driven Development works in complex, real-world scenarios!

---

*Back to: [Lesson 19: Iterative Enhancement (Brownfield)](./Lesson-19-Iterative-Enhancement-Brownfield.md)*  
*Next: Module 6 - [Lesson 20: Enterprise Considerations](../Module-06-Real-World-Application/Lesson-20-Enterprise-Considerations.md)*
