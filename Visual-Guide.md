# 📊 Visual Guide to Spec-Driven Development

This document contains all the key diagrams and visual explanations for Spec-Driven Development concepts.

---

## 🔄 The Complete Workflow

```mermaid
graph TB
    Start([Start New Feature]) --> Init[Initialize Project<br/>specify init]
    
    Init --> Constitution[Step 1: Constitution<br/>/speckit.constitution<br/>Define Principles]
    
    Constitution --> Specify[Step 2: Specify<br/>/speckit.specify<br/>What & Why]
    
    Specify --> Optional1{Optional:<br/>Clarify?}
    Optional1 -->|Yes| Clarify[/speckit.clarify<br/>Refine Specs]
    Optional1 -->|No| Plan
    Clarify --> Plan[Step 3: Plan<br/>/speckit.plan<br/>Tech Stack & Architecture]
    
    Plan --> Tasks[Step 4: Tasks<br/>/speckit.tasks<br/>Break Down Work]
    
    Tasks --> Optional2{Optional:<br/>Analyze?}
    Optional2 -->|Yes| Analyze[/speckit.analyze<br/>Consistency Check]
    Optional2 -->|No| Implement
    Analyze --> Implement[Step 5: Implement<br/>/speckit.implement<br/>Execute Tasks]
    
    Implement --> Optional3{Optional:<br/>Checklist?}
    Optional3 -->|Yes| Checklist[/speckit.checklist<br/>Quality Validation]
    Optional3 -->|No| Test
    Checklist --> Test[Step 6: Validate<br/>Test & Review]
    
    Test --> Decision{Satisfactory?}
    Decision -->|No, needs changes| Specify
    Decision -->|Yes| Done([Feature Complete])
    
    style Constitution fill:#e8f5e9
    style Specify fill:#fff9c4
    style Plan fill:#fff3e0
    style Tasks fill:#fce4ec
    style Implement fill:#e1f5fe
    style Test fill:#f3e5f5
    style Clarify fill:#ffe082
    style Analyze fill:#81c784
    style Checklist fill:#64b5f6
```

---

## 🆚 Traditional vs Spec-Driven: Side-by-Side

```mermaid
graph TB
    subgraph Traditional["❌ Traditional Development"]
        T1[Business Requirements] --> T2[Design Document]
        T2 --> T3[Spec Document<br/>Often incomplete]
        T3 --> T4[Developer Reads Spec]
        T4 --> T5[Developer Writes Code]
        T5 --> T6[Spec Becomes Outdated]
        T6 --> T7[Code is Truth]
        
        T7 -.Need Change?.-> T8[Modify Code Directly]
        T8 --> T9[Hope Docs Updated<br/>Usually aren't]
        
        style T6 fill:#ffcdd2
        style T9 fill:#ffcdd2
    end
    
    subgraph SpecDriven["✅ Spec-Driven Development"]
        S1[Business Requirements] --> S2[Rich Specifications<br/>Detailed & Precise]
        S2 --> S3[AI Interprets Spec]
        S3 --> S4[AI Generates Code]
        S4 --> S5[Spec Stays Current]
        S5 --> S6[Spec is Truth]
        
        S6 -.Need Change?.-> S7[Update Specification]
        S7 --> S8[Regenerate Code<br/>Always in Sync]
        S8 --> S5
        
        style S5 fill:#c8e6c9
        style S8 fill:#c8e6c9
    end
```

---

## 🎭 Roles & Responsibilities

```mermaid
graph LR
    subgraph Human["👤 Human Developer"]
        direction TB
        H1[Creative Thinking]
        H2[Business Logic]
        H3[User Experience]
        H4[Architecture Decisions]
        H5[Quality Standards]
        H6[Specification Writing]
    end
    
    subgraph Specs["📄 Specifications"]
        direction TB
        SP1[Requirements]
        SP2[User Stories]
        SP3[Acceptance Criteria]
        SP4[Edge Cases]
    end
    
    subgraph AI["🤖 AI Assistant"]
        direction TB
        A1[Code Generation]
        A2[Consistency Checking]
        A3[Boilerplate Creation]
        A4[Test Generation]
        A5[Documentation]
        A6[Refactoring]
    end
    
    subgraph Code["💻 Implementation"]
        direction TB
        C1[Working Code]
        C2[Tests]
        C3[Documentation]
        C4[Best Practices]
    end
    
    Human -->|Writes| Specs
    Specs -->|Feeds| AI
    AI -->|Generates| Code
    Code -->|Validates| Human
    
    style Human fill:#e3f2fd
    style Specs fill:#fff9c4
    style AI fill:#fff3e0
    style Code fill:#f3e5f5
```

---

## 📈 Information Flow Through the Workflow

```mermaid
graph TD
    Constitution[Constitution<br/>Principles & Standards]
    
    Constitution ==> Spec[Specification<br/>WHAT to build<br/>WHY it matters]
    
    Spec ==> Plan[Implementation Plan<br/>HOW to build it<br/>Tech choices]
    
    Plan ==> Tasks[Task List<br/>Step-by-step actions<br/>Dependencies]
    
    Tasks ==> Code[Generated Code<br/>Working implementation<br/>Tests & docs]
    
    Code -.Feedback.-> Spec
    Constitution -.Guides.-> Plan
    Constitution -.Validates.-> Code
    
    style Constitution fill:#e8f5e9,stroke:#2e7d32,stroke-width:3px
    style Spec fill:#fff9c4,stroke:#f57f17,stroke-width:3px
    style Plan fill:#fff3e0,stroke:#e65100,stroke-width:3px
    style Tasks fill:#fce4ec,stroke:#c2185b,stroke-width:3px
    style Code fill:#e1f5fe,stroke:#0277bd,stroke-width:3px
```

---

## 🔍 Specification Lifecycle

```mermaid
stateDiagram-v2
    [*] --> Draft: Create initial spec
    
    Draft --> UnderReview: Submit for clarification
    UnderReview --> Draft: Needs refinement
    UnderReview --> Approved: Clear and complete
    
    Approved --> Planned: Create implementation plan
    Planned --> TaskBrokenDown: Generate tasks
    TaskBrokenDown --> InProgress: Start implementation
    
    InProgress --> Testing: Code generated
    Testing --> InProgress: Issues found
    Testing --> Deployed: All tests pass
    
    Deployed --> [*]: Feature complete
    Deployed --> Draft: New requirements<br/>(iteration)
    
    note right of Approved
        Spec remains the
        source of truth
    end note
    
    note right of InProgress
        Code generated
        from spec
    end note
```

---

## 🌳 Project Structure (Feature Branches)

```mermaid
graph TD
    Main[main branch<br/>Stable code]
    
    Main --> Feature1[feature/001-photo-albums<br/>Constitution + Specs + Plan + Tasks]
    Main --> Feature2[feature/002-user-auth<br/>Constitution + Specs + Plan + Tasks]
    Main --> Feature3[feature/003-sharing<br/>Constitution + Specs + Plan + Tasks]
    
    Feature1 --> Impl1[Implementation<br/>Generated Code]
    Feature2 --> Impl2[Implementation<br/>Generated Code]
    Feature3 --> Impl3[Implementation<br/>Generated Code]
    
    Impl1 -.Merge when complete.-> Main
    Impl2 -.Merge when complete.-> Main
    Impl3 -.Merge when complete.-> Main
    
    style Main fill:#4caf50,color:#fff
    style Feature1 fill:#2196f3,color:#fff
    style Feature2 fill:#2196f3,color:#fff
    style Feature3 fill:#2196f3,color:#fff
```

---

## 🎯 Quality Assurance Flow

```mermaid
graph LR
    Input[Requirements] --> Clarify{Clarify<br/>underspecified<br/>areas?}
    
    Clarify -->|Yes| ClarifyProcess[/speckit.clarify<br/>Socratic questioning]
    Clarify -->|No| Spec[Create Spec]
    ClarifyProcess --> Spec
    
    Spec --> Checklist1[/speckit.checklist<br/>Validate requirements]
    Checklist1 --> Plan[Create Plan]
    
    Plan --> Tasks[Generate Tasks]
    Tasks --> Analyze[/speckit.analyze<br/>Consistency check]
    
    Analyze --> Implement[Implement]
    Implement --> Checklist2[/speckit.checklist<br/>Quality validation]
    
    Checklist2 --> Output[Quality Output]
    
    style ClarifyProcess fill:#ffe082
    style Checklist1 fill:#64b5f6
    style Analyze fill:#81c784
    style Checklist2 fill:#64b5f6
    style Output fill:#aed581
```

---

## 💡 The AI Partnership Model

```mermaid
graph TB
    subgraph Partnership["Human-AI Partnership"]
        direction LR
        
        subgraph HumanZone["Human Expertise Zone"]
            H1[Problem Definition]
            H2[Creative Solutions]
            H3[User Empathy]
            H4[Business Context]
            H5[Ethical Decisions]
        end
        
        subgraph SharedZone["Collaborative Zone"]
            SH1[Architecture Design]
            SH2[API Design]
            SH3[Testing Strategy]
            SH4[Code Review]
        end
        
        subgraph AIZone["AI Expertise Zone"]
            A1[Code Generation]
            A2[Boilerplate Creation]
            A3[Syntax & Patterns]
            A4[Documentation]
            A5[Consistency Checking]
        end
        
        HumanZone <--> SharedZone
        SharedZone <--> AIZone
    end
    
    style HumanZone fill:#e3f2fd
    style SharedZone fill:#fff9c4
    style AIZone fill:#fff3e0
```

---

## 🔄 Iteration & Feedback Loop

```mermaid
graph TD
    Start([Start]) --> Spec1[Initial Specification<br/>v1.0]
    
    Spec1 --> Impl1[Implementation<br/>v1.0]
    Impl1 --> Test1[Testing & Feedback]
    
    Test1 --> Decision1{Issues Found?}
    Decision1 -->|Yes| UpdateSpec1[Update Specification<br/>v1.1]
    Decision1 -->|No| Success1[Feature Complete]
    
    UpdateSpec1 --> Impl2[Regenerate Implementation<br/>v1.1]
    Impl2 --> Test2[Testing & Feedback]
    
    Test2 --> Decision2{Issues Found?}
    Decision2 -->|Yes| UpdateSpec2[Update Specification<br/>v1.2]
    Decision2 -->|No| Success2[Feature Complete]
    
    UpdateSpec2 --> Impl3[Regenerate Implementation<br/>v1.2]
    Impl3 --> Success3[Feature Complete]
    
    Success1 --> End([Done])
    Success2 --> End
    Success3 --> End
    
    style Spec1 fill:#fff9c4
    style UpdateSpec1 fill:#fff9c4
    style UpdateSpec2 fill:#fff9c4
    style Impl1 fill:#e1f5fe
    style Impl2 fill:#e1f5fe
    style Impl3 fill:#e1f5fe
    style Success1 fill:#c8e6c9
    style Success2 fill:#c8e6c9
    style Success3 fill:#c8e6c9
```

---

## 🎨 Three Development Phases in Detail

```mermaid
graph TB
    Choice{Choose Your<br/>Development Phase}
    
    Choice -->|New Project| Greenfield[0-to-1 Greenfield]
    Choice -->|Explore Options| Creative[Creative Exploration]
    Choice -->|Existing Code| Brownfield[Iterative Enhancement]
    
    Greenfield --> GF1[Empty Canvas]
    GF1 --> GF2[Constitution]
    GF2 --> GF3[Full Specs]
    GF3 --> GF4[Complete Plan]
    GF4 --> GF5[Full Implementation]
    GF5 --> GFResult[New Application]
    
    Creative --> CR1[Same Spec]
    CR1 --> CR2[Multiple Plans]
    CR2 --> CR3[Plan A:<br/>React + Node]
    CR2 --> CR4[Plan B:<br/>Vue + Python]
    CR2 --> CR5[Plan C:<br/>Svelte + Go]
    CR3 --> CRResult[Compare & Choose]
    CR4 --> CRResult
    CR5 --> CRResult
    
    Brownfield --> BF1[Existing Codebase]
    BF1 --> BF2[New Feature Spec]
    BF2 --> BF3[Integration Plan]
    BF3 --> BF4[Incremental Tasks]
    BF4 --> BF5[Careful Implementation]
    BF5 --> BFResult[Enhanced Application]
    
    style Greenfield fill:#a5d6a7
    style Creative fill:#ffcc80
    style Brownfield fill:#90caf9
    style GFResult fill:#81c784
    style CRResult fill:#ffb74d
    style BFResult fill:#64b5f6
```

---

## 🧩 How Specifications Become Code

```mermaid
sequenceDiagram
    participant Developer
    participant Specification
    participant AI
    participant Code
    
    Developer->>Specification: Write detailed spec<br/>(What & Why)
    Specification->>AI: Parse requirements
    AI->>AI: Understand intent
    AI->>AI: Consider tech stack
    AI->>AI: Apply best practices
    AI->>Code: Generate implementation
    Code->>Developer: Review generated code
    
    Developer->>Specification: Request change
    Specification->>AI: Updated requirements
    AI->>Code: Regenerate affected parts
    Code->>Developer: Updated implementation
    
    Note over Developer,Code: Spec remains source of truth
```

---

## 📊 Comparison: One-Shot vs Multi-Step

```mermaid
graph TB
    subgraph OneShot["One-Shot Prompting (Traditional AI)"]
        OS1[Single Prompt:<br/>'Build me a photo app'] --> OS2[AI Generates Code]
        OS2 --> OS3{Good Enough?}
        OS3 -->|No| OS4[Write New Prompt]
        OS3 -->|Yes| OS5[Done]
        OS4 --> OS2
        
        style OS3 fill:#ffcdd2
        note1[Problem: Unclear intent,<br/>inconsistent results,<br/>hard to iterate]
    end
    
    subgraph MultiStep["Multi-Step Spec-Driven"]
        MS1[Step 1: Constitution] --> MS2[Step 2: Detailed Spec]
        MS2 --> MS3[Step 3: Technical Plan]
        MS3 --> MS4[Step 4: Task Breakdown]
        MS4 --> MS5[Step 5: Implementation]
        MS5 --> MS6[Step 6: Validation]
        MS6 --> MS7{Satisfactory?}
        MS7 -->|No| MS8[Refine Spec]
        MS7 -->|Yes| MS9[Done]
        MS8 --> MS2
        
        style MS7 fill:#c8e6c9
        note2[Benefit: Clear intent,<br/>consistent results,<br/>easy to iterate]
    end
```

---

## 🎓 Learning Path Visualization

```mermaid
graph LR
    Start([Beginner]) --> M1[Module 1:<br/>Foundations]
    M1 --> M2[Module 2:<br/>Getting Started]
    M2 --> M3[Module 3:<br/>Core Workflow]
    M3 --> M4[Module 4:<br/>Advanced Techniques]
    M4 --> M5[Module 5:<br/>Development Phases]
    M5 --> M6[Module 6:<br/>Real-World Application]
    M6 --> M7[Module 7:<br/>Mastery]
    M7 --> End([Expert])
    
    M3 -.Practice.-> Practice1[Hands-on Projects]
    M4 -.Practice.-> Practice1
    M5 -.Practice.-> Practice1
    
    Practice1 --> Capstone[Capstone Project]
    Capstone --> End
    
    style Start fill:#ffcdd2
    style M3 fill:#fff9c4
    style M4 fill:#fff3e0
    style M5 fill:#e1f5fe
    style Practice1 fill:#c8e6c9
    style Capstone fill:#ce93d8
    style End fill:#a5d6a7
```

---

## 🔧 CLI Commands Flow

```mermaid
graph TD
    Install[Install: uv tool install<br/>specify-cli]
    
    Install --> Check[Check Prerequisites:<br/>specify check]
    
    Check --> Init[Initialize Project:<br/>specify init my-project<br/>--ai copilot]
    
    Init --> Structure[Project Structure Created]
    
    Structure --> Git[Git Repository<br/>Initialized]
    
    Git --> Feature[Create Feature Branch:<br/>git checkout -b<br/>feature/001-my-feature]
    
    Feature --> SlashCommands[Use Slash Commands:<br/>/speckit.constitution<br/>/speckit.specify<br/>/speckit.plan<br/>etc.]
    
    SlashCommands --> Implement[Implementation Generated]
    
    Implement --> Merge[Merge to Main:<br/>git merge]
    
    Merge --> Next{Another Feature?}
    Next -->|Yes| Feature
    Next -->|No| Done([Project Complete])
    
    style Install fill:#e3f2fd
    style Check fill:#fff9c4
    style Init fill:#fff3e0
    style SlashCommands fill:#f3e5f5
    style Done fill:#c8e6c9
```

---

*Use these diagrams as visual references throughout your learning journey!*
