# Final Capstone Project Guide

**Spec Kit Course - Final Assessment**  
**Date:** November 29, 2025  
**Version:** 1.0

---

## Overview

The capstone project is your opportunity to demonstrate mastery of spec-driven development. You'll take a real or realistic project through the entire Spec Kit workflow, from constitution to implementation, showcasing everything you've learned.

**Duration:** 4-6 weeks (part-time) or 2-3 weeks (full-time)  
**Complexity:** Equivalent to a medium-sized feature or small application  
**Deliverables:** Complete Spec Kit artifact set + working implementation

---

## Learning Objectives

By completing the capstone, you will:
- Apply the entire Spec Kit workflow to a realistic project
- Create production-quality specifications
- Integrate AI agents effectively
- Demonstrate user-centric design
- Showcase technical and communication skills
- Build a portfolio piece

---

## Project Requirements

### Core Requirements (Must Complete)

1. **Complete Artifact Set:**
   - [ ] Constitution (project principles and constraints)
   - [ ] At least 3 detailed specifications
   - [ ] At least 3 implementation plans
   - [ ] At least 3 task breakdowns
   - [ ] Checklist tracking

2. **Working Implementation:**
   - [ ] Functional software that meets specifications
   - [ ] Comprehensive tests (unit, integration, or E2E as appropriate)
   - [ ] Documentation (README, API docs, etc.)
   - [ ] Deployed or deployable

3. **AI Integration:**
   - [ ] Evidence of AI agent usage (prompts, outputs)
   - [ ] Reflection on what worked and what didn't
   - [ ] Comparison: with vs. without AI

4. **User-Centric Design:**
   - [ ] User research or persona definition
   - [ ] Accessibility considerations (WCAG AA)
   - [ ] User validation (prototype testing, usability testing, or user feedback)

5. **Quality & Professionalism:**
   - [ ] Clean code (follows best practices)
   - [ ] Git history (meaningful commits)
   - [ ] Professional presentation

### Advanced Requirements (Optional, for Distinction)

Choose 1-2 to demonstrate depth:

- [ ] **Formal Verification:** Use TLA+ or similar to prove critical properties
- [ ] **Enterprise Features:** Authentication, authorization, audit logging, multi-tenancy
- [ ] **Performance:** Demonstrate optimization with before/after metrics
- [ ] **Internationalization:** Support multiple languages
- [ ] **Advanced AI:** Multi-agent implementation or AI-assisted optimization
- [ ] **Research Component:** Experiment with novel spec-driven techniques
- [ ] **Open Source:** Publish as open source with community engagement

---

## Project Options

### Option 1: Build a New Feature (Recommended for Most)

**Choose One:**

#### A. Task Management System
**Description:** Build a task/project management tool (e.g., mini Trello, Asana)

**Core Features:**
- User authentication
- Project creation and management
- Task creation, assignment, and status tracking
- Basic collaboration (comments, mentions)

**User Cohorts:**
- Solo users (personal productivity)
- Small teams (3-5 people)

**Constraints:**
- Must work on mobile
- <2s page load time
- Offline-first (optional advanced feature)

**Success Criteria:**
- User can create and complete a task in <30 seconds
- Team can collaborate on a project
- 90%+ uptime

---

#### B. API Documentation Generator
**Description:** Generate beautiful, interactive API documentation from OpenAPI specs

**Core Features:**
- Parse OpenAPI/Swagger files
- Generate interactive documentation
- Try-it-out functionality (test API calls in browser)
- Search and filtering

**User Cohorts:**
- API developers (create docs)
- API consumers (read and test APIs)

**Constraints:**
- Support OpenAPI 3.0
- Accessibility: WCAG AA
- Mobile-responsive

**Success Criteria:**
- Generate docs for 100+ endpoint API in <5 seconds
- User can test API calls directly from docs
- Search finds relevant endpoints in <1 second

---

#### C. Personal Finance Dashboard
**Description:** Visualize and track personal finances

**Core Features:**
- Transaction import (CSV or manual entry)
- Categorization (automatic or manual)
- Budget tracking
- Visualizations (spending over time, category breakdown)

**User Cohorts:**
- Young professionals (25-35)
- Budget-conscious individuals
- Visual learners

**Constraints:**
- Privacy-first (local data storage or encrypted cloud)
- Mobile-friendly
- Accessible to screen reader users

**Success Criteria:**
- User can import 100 transactions in <30 seconds
- Visualizations load in <1 second
- Budget tracking updates real-time

---

#### D. Markdown-Based Wiki
**Description:** Knowledge base system using Markdown files

**Core Features:**
- Create, edit, and organize markdown pages
- Full-text search
- Linking between pages
- Version history (via Git)

**User Cohorts:**
- Technical writers
- Development teams (internal docs)
- Knowledge managers

**Constraints:**
- Files stored as plain markdown (future-proof)
- Fast search (<500ms for 1000+ pages)
- Keyboard shortcuts for power users

**Success Criteria:**
- User can create new page in <10 seconds
- Search finds relevant pages quickly
- Links between pages are intuitive

---

### Option 2: Modernize Legacy Code

**Challenge:** Take an existing codebase (your own or open source) and modernize it using Spec Kit.

**Steps:**
1. **Analyze Legacy System:**
   - Document current behavior
   - Identify pain points
   - Map dependencies

2. **Specify Desired Behavior:**
   - Write specs for what the system should do
   - Highlight differences from current state
   - Prioritize modernization areas

3. **Plan Migration:**
   - Use Strangler Fig pattern
   - Phase the migration
   - Define rollback procedures

4. **Implement:**
   - Refactor using modern practices
   - Maintain backward compatibility (where needed)
   - Comprehensive testing

**Deliverables:**
- Legacy analysis document
- Modernization specs
- Migration plan
- Refactored code
- Comparison metrics (performance, maintainability, test coverage)

---

### Option 3: Open Source Contribution

**Challenge:** Make a significant contribution to an open source project using Spec Kit workflow.

**Steps:**
1. **Choose Project:**
   - Find open source project you use or care about
   - Identify feature or improvement needed

2. **Collaborate:**
   - Discuss with maintainers
   - Get alignment on approach

3. **Spec-Driven Development:**
   - Write specification for contribution
   - Get feedback from maintainers
   - Plan implementation
   - Break down tasks

4. **Implement & Submit:**
   - Develop feature
   - Comprehensive tests
   - Documentation
   - Submit PR with spec

**Deliverables:**
- Full spec-kit artifact set
- Merged PR (or substantive feedback from maintainers)
- Reflection on collaboration process

---

### Option 4: Create Your Own

**Requirements:**
- Similar complexity to provided options
- Addresses a real need (yours or others')
- Demonstrates full Spec Kit workflow
- Get approval from instructor/mentor before starting

**Proposal Template:**
```markdown
## Capstone Project Proposal

**Title:** [Project name]

**Problem Statement:**
[What problem does this solve? For whom?]

**Core Features:** (3-5)
1. [Feature 1]
2. [Feature 2]
3. [Feature 3]

**User Cohorts:** (2-3)
- [Cohort 1]: [Description]
- [Cohort 2]: [Description]

**Technical Approach:**
- Language/Framework: [Choice]
- Database: [Choice]
- Deployment: [How you'll deploy]

**Complexity Justification:**
[Why this is equivalent to provided options]

**Timeline:**
- Week 1: [Milestones]
- Week 2: [Milestones]
- Week 3: [Milestones]
- Week 4: [Milestones]

**Success Criteria:**
- [How you'll measure success]
```

---

## Detailed Requirements by Artifact

### 1. Constitution (CONSTITUTION.md)

**Must Include:**
- Project name and vision
- Core principles (3-5)
- Technology constraints
- Quality standards
- Non-negotiables
- Success definition

**Example:**
```markdown
# Constitution: TaskFlow

## Vision
A task management system that's fast, accessible, and delightful.

## Core Principles
1. **User First:** Every feature must serve user needs
2. **Speed:** Sub-second interactions
3. **Accessibility:** WCAG AA compliance, minimum
4. **Privacy:** User data is sacred
5. **Simplicity:** Complex features, simple interface

## Technology Constraints
- Frontend: React + TypeScript
- Backend: Node.js + Express
- Database: PostgreSQL
- Deployment: Vercel
- AI Assistance: GitHub Copilot, ChatGPT

## Quality Standards
- Test coverage: >80%
- Accessibility: WCAG AA, Lighthouse score >90
- Performance: Lighthouse score >90
- Code quality: ESLint, Prettier

## Non-Negotiables
- No user tracking without consent
- Mobile-first design
- Keyboard accessible
- Data export (user owns their data)

## Success Criteria
- 10 test users complete core workflows successfully
- Performance targets met
- Accessibility audit passes
- Personal satisfaction with quality
```

---

### 2. Specifications (SPECS/)

**Minimum: 3 detailed specifications**

**Must Include Per Spec:**
- User story or problem statement
- Functional requirements (clear, testable)
- Non-functional requirements (performance, security, etc.)
- Acceptance criteria
- Testing approach
- Success metrics

**Quality Standards:**
- Unambiguous (no "should", "might", "approximately")
- Testable (can you write tests from this?)
- Complete (covers happy path, edge cases, errors)
- Consistent (no contradictions)
- User-focused (why does this matter?)

**Example Specification:**
```markdown
# SPEC-001: User Authentication

## User Story
As a user, I want to create an account and log in securely so I can access my tasks from any device.

## Functional Requirements

### 1. Registration (REQ-AUTH-REG-001)
**Inputs:**
- Email: RFC 5322 compliant
- Password: Min 12 characters, must include uppercase, lowercase, number, symbol
- Name: 2-50 characters

**Process:**
1. Validate inputs (client-side and server-side)
2. Check email uniqueness
3. Hash password (bcrypt, cost factor 12)
4. Create user record
5. Send verification email

**Outputs:**
- Success: User record created, verification email sent
- Failure: Error message (specific, not revealing)

### 2. Login (REQ-AUTH-LOGIN-001)
**Inputs:**
- Email
- Password

**Process:**
1. Rate limiting: 5 attempts per 15 minutes per IP
2. Lookup user by email
3. Compare password (bcrypt)
4. Create session (JWT, 7-day expiry)
5. Return session token

**Outputs:**
- Success: JWT token, redirect to dashboard
- Failure: "Invalid credentials" (don't reveal which field)

### 3. Session Management (REQ-AUTH-SESSION-001)
- Session stored in HTTP-only, secure cookie
- Sliding window: Extend session on activity
- Logout: Invalidate session server-side
- View active sessions: List devices, locations

## Non-Functional Requirements

**Security:**
- HTTPS only
- CSRF protection
- XSS prevention
- Password hashing: bcrypt cost 12
- Rate limiting: Prevent brute force

**Performance:**
- Login: <500ms (p95)
- Registration: <1s (p95)
- Session validation: <100ms (p95)

**Accessibility:**
- Form labels clearly associated
- Error messages descriptive
- Keyboard navigable
- Screen reader friendly

## Acceptance Criteria

- [ ] User can register with valid credentials
- [ ] User cannot register with weak password
- [ ] User cannot register with duplicate email
- [ ] User receives verification email
- [ ] User can log in with valid credentials
- [ ] User cannot log in with invalid credentials
- [ ] Session persists across page reloads
- [ ] Session expires after 7 days of inactivity
- [ ] User can log out
- [ ] Rate limiting prevents brute force (test with 10 rapid attempts)
- [ ] OWASP ZAP security scan: 0 high/medium vulnerabilities

## Testing Approach

**Unit Tests:**
- Password validation logic
- Email validation logic
- Password hashing and comparison

**Integration Tests:**
- Registration flow (happy path)
- Registration flow (validation errors)
- Login flow (happy path)
- Login flow (invalid credentials)
- Session management (create, validate, expire)

**Security Tests:**
- OWASP ZAP automated scan
- Manual penetration testing (SQL injection, XSS, CSRF)

**Accessibility Tests:**
- Axe-core (0 violations)
- Screen reader testing (NVDA, VoiceOver)
- Keyboard navigation

## Success Metrics

**Primary:**
- Registration completion rate: >80%
- Login success rate: >95% (for valid users)
- Security issues: 0 critical, 0 high

**Secondary:**
- Registration time (median): <2 minutes
- Login time (median): <30 seconds
- User satisfaction: 4+ out of 5
```

---

### 3. Implementation Plans (PLANS/)

**Minimum: 3 plans (one per spec)**

**Must Include:**
- Reference to specification
- Technical approach
- Technology choices (with rationale)
- Architecture (diagram)
- Data models
- API design (if applicable)
- Key algorithms or logic
- Error handling
- Testing strategy

**Example Plan:**
```markdown
# PLAN-001: User Authentication Implementation

**Specification:** SPEC-001: User Authentication

## Technical Approach

### Architecture

```
┌─────────────┐      ┌──────────────┐      ┌──────────────┐
│   Client    │─────▶│   API Server │─────▶│  PostgreSQL  │
│  (React)    │◀─────│  (Node/Express)│◀─────│   Database   │
└─────────────┘      └──────────────┘      └──────────────┘
       │                     │
       │                     │
       └─────────────────────▼
                    ┌──────────────┐
                    │ Redis (Sessions)│
                    └──────────────┘
```

### Technology Stack

**Frontend:**
- React: UI components
- React Router: Navigation
- Axios: API calls
- React Hook Form: Form handling + validation

**Backend:**
- Node.js + Express: API server
- bcrypt: Password hashing
- jsonwebtoken: JWT generation/validation
- express-rate-limit: Rate limiting
- joi: Input validation

**Database:**
- PostgreSQL: User data
- Redis: Session storage

**Rationale:**
- React: Team familiarity, component reusability
- Node: JavaScript full-stack, large ecosystem
- PostgreSQL: ACID compliance, relational data
- Redis: Fast session lookup

### Data Models

**User Table (PostgreSQL):**
```sql
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  email VARCHAR(255) UNIQUE NOT NULL,
  password_hash VARCHAR(255) NOT NULL,
  name VARCHAR(100) NOT NULL,
  email_verified BOOLEAN DEFAULT FALSE,
  created_at TIMESTAMP DEFAULT NOW(),
  updated_at TIMESTAMP DEFAULT NOW()
);

CREATE INDEX idx_users_email ON users(email);
```

**Session Table (Redis):**
```
Key: session:{sessionId}
Value: {
  userId: UUID,
  createdAt: timestamp,
  expiresAt: timestamp,
  ipAddress: string,
  userAgent: string
}
TTL: 7 days (auto-expires)
```

### API Endpoints

**POST /api/auth/register**
```json
Request:
{
  "email": "user@example.com",
  "password": "SecureP@ssw0rd",
  "name": "John Doe"
}

Response (201):
{
  "success": true,
  "message": "Registration successful. Please check your email."
}

Response (400):
{
  "success": false,
  "errors": [
    {"field": "password", "message": "Password must be at least 12 characters"}
  ]
}
```

**POST /api/auth/login**
```json
Request:
{
  "email": "user@example.com",
  "password": "SecureP@ssw0rd"
}

Response (200):
{
  "success": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...",
  "user": {
    "id": "uuid",
    "email": "user@example.com",
    "name": "John Doe"
  }
}

Response (401):
{
  "success": false,
  "message": "Invalid credentials"
}
```

### Key Implementation Details

**Password Hashing:**
```javascript
const bcrypt = require('bcrypt');
const SALT_ROUNDS = 12;

async function hashPassword(password) {
  return await bcrypt.hash(password, SALT_ROUNDS);
}

async function comparePassword(password, hash) {
  return await bcrypt.compare(password, hash);
}
```

**Rate Limiting:**
```javascript
const rateLimit = require('express-rate-limit');

const loginLimiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 5, // 5 attempts
  message: 'Too many login attempts. Please try again later.',
  standardHeaders: true,
  legacyHeaders: false,
});

app.post('/api/auth/login', loginLimiter, loginHandler);
```

**JWT Generation:**
```javascript
const jwt = require('jsonwebtoken');

function generateToken(userId) {
  return jwt.sign(
    { userId },
    process.env.JWT_SECRET,
    { expiresIn: '7d' }
  );
}

function verifyToken(token) {
  return jwt.verify(token, process.env.JWT_SECRET);
}
```

### Error Handling

**Validation Errors:**
- Return 400 with specific field errors
- Client displays inline error messages

**Authentication Errors:**
- Return 401 with generic message
- Don't reveal whether email or password was wrong (security)

**Server Errors:**
- Return 500 with generic message
- Log detailed error server-side
- Alert monitoring system

### Testing Strategy

**Unit Tests (Jest):**
- Password validation functions
- Email validation functions
- Token generation/verification
- Password hashing/comparison

**Integration Tests (Supertest):**
- Registration API endpoint
- Login API endpoint
- Session validation endpoint
- Error scenarios

**Security Tests:**
- OWASP ZAP scan
- Manual SQL injection attempts
- XSS attempts
- CSRF testing

**E2E Tests (Cypress):**
- User registration flow
- User login flow
- Session persistence
- Logout flow

## Implementation Tasks

*(See TASKS/TASK-001-*.md for breakdown)*

1. Database schema and migrations
2. User model and data access layer
3. Password hashing utilities
4. JWT utilities
5. Registration endpoint
6. Login endpoint
7. Session validation middleware
8. Rate limiting middleware
9. Frontend registration form
10. Frontend login form
11. Session management (client-side)
12. Testing (unit, integration, E2E)
13. Security hardening
14. Documentation
```

---

### 4. Task Breakdowns (TASKS/)

**Minimum: 3 task sets (one per plan)**

**Must Include Per Task:**
- Task ID
- Description (what to do)
- Acceptance criteria (when it's done)
- Estimated effort
- Dependencies
- Implementation notes
- Testing requirements

**Example Tasks:**
```markdown
# TASK-001-01: Database Schema and Migrations

**Plan:** PLAN-001: User Authentication  
**Estimated Effort:** 2 hours  
**Dependencies:** None (first task)

## Description

Create PostgreSQL database schema for users table and set up migration system.

## Acceptance Criteria

- [ ] Users table created with all required columns
- [ ] Indexes created (email)
- [ ] Migration system set up (e.g., node-pg-migrate)
- [ ] Up/down migrations working
- [ ] Seed data for testing (3 test users)

## Implementation Notes

**Migration Tool:** `node-pg-migrate`

**Schema:**
```sql
-- migrations/001_create_users_table.sql
CREATE EXTENSION IF NOT EXISTS "pgcrypto";

CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  email VARCHAR(255) UNIQUE NOT NULL,
  password_hash VARCHAR(255) NOT NULL,
  name VARCHAR(100) NOT NULL,
  email_verified BOOLEAN DEFAULT FALSE,
  created_at TIMESTAMP DEFAULT NOW(),
  updated_at TIMESTAMP DEFAULT NOW()
);

CREATE INDEX idx_users_email ON users(email);
```

**Rollback:**
```sql
DROP TABLE IF EXISTS users;
```

**Seed Data:**
```sql
-- seeds/test_users.sql
INSERT INTO users (email, password_hash, name, email_verified)
VALUES
  ('test1@example.com', '$2b$12$...', 'Test User 1', true),
  ('test2@example.com', '$2b$12$...', 'Test User 2', true),
  ('test3@example.com', '$2b$12$...', 'Test User 3', false);
```

## Testing

**Manual Test:**
1. Run migration: `npm run migrate up`
2. Verify table exists: `psql -d dbname -c "\d users"`
3. Verify indexes: `psql -d dbname -c "\di"`
4. Run rollback: `npm run migrate down`
5. Verify table removed

**Automated Test:**
```javascript
// tests/database/migrations.test.js
describe('User table migration', () => {
  it('creates users table with correct schema', async () => {
    const result = await db.query(`
      SELECT column_name, data_type, is_nullable
      FROM information_schema.columns
      WHERE table_name = 'users'
    `);
    
    expect(result.rows).toContainEqual({
      column_name: 'id',
      data_type: 'uuid',
      is_nullable: 'NO'
    });
    // ... more assertions
  });
});
```

---

# TASK-001-02: User Model and Data Access Layer

**Plan:** PLAN-001: User Authentication  
**Estimated Effort:** 3 hours  
**Dependencies:** TASK-001-01 (database schema)

## Description

Create User model with methods for CRUD operations and authentication-related queries.

## Acceptance Criteria

- [ ] User model class created
- [ ] Methods: create, findByEmail, findById, update, delete
- [ ] Error handling for duplicate email
- [ ] Connection pooling configured
- [ ] Unit tests for all methods (>90% coverage)

## Implementation Notes

**File:** `src/models/User.js`

```javascript
const pool = require('../database/pool');

class User {
  static async create({ email, passwordHash, name }) {
    const result = await pool.query(
      `INSERT INTO users (email, password_hash, name)
       VALUES ($1, $2, $3)
       RETURNING id, email, name, created_at`,
      [email, passwordHash, name]
    );
    return result.rows[0];
  }

  static async findByEmail(email) {
    const result = await pool.query(
      'SELECT * FROM users WHERE email = $1',
      [email]
    );
    return result.rows[0];
  }

  static async findById(id) {
    const result = await pool.query(
      'SELECT id, email, name, email_verified, created_at FROM users WHERE id = $1',
      [id]
    );
    return result.rows[0];
  }

  static async update(id, fields) {
    // Dynamic update based on fields provided
    // ...
  }

  static async delete(id) {
    await pool.query('DELETE FROM users WHERE id = $1', [id]);
  }
}

module.exports = User;
```

**Error Handling:**
- Catch duplicate email error (PostgreSQL error code 23505)
- Throw custom `DuplicateEmailError`

## Testing

```javascript
// tests/models/User.test.js
describe('User model', () => {
  beforeEach(async () => {
    await pool.query('TRUNCATE users CASCADE');
  });

  describe('create', () => {
    it('creates a new user with valid data', async () => {
      const user = await User.create({
        email: 'test@example.com',
        passwordHash: 'hashed_password',
        name: 'Test User'
      });

      expect(user).toHaveProperty('id');
      expect(user.email).toBe('test@example.com');
    });

    it('throws error for duplicate email', async () => {
      await User.create({
        email: 'duplicate@example.com',
        passwordHash: 'hash1',
        name: 'User 1'
      });

      await expect(
        User.create({
          email: 'duplicate@example.com',
          passwordHash: 'hash2',
          name: 'User 2'
        })
      ).rejects.toThrow('Email already exists');
    });
  });

  // More tests...
});
```

---

*(Continue for all tasks in the authentication feature...)*
```

---

### 5. Implementation & Testing

**Must Include:**

**Code:**
- Clean, readable code
- Comments where complex logic exists
- Follows language/framework conventions
- No hardcoded secrets (use environment variables)

**Tests:**
- Unit tests (business logic)
- Integration tests (API endpoints, database interactions)
- E2E tests (critical user flows) OR manual testing documentation
- >80% code coverage (or justify lower)

**Documentation:**
- README with setup instructions
- API documentation (if applicable)
- Architecture overview
- Deployment guide

**Example README:**
```markdown
# TaskFlow - Task Management System

Simple, fast, accessible task management for individuals and small teams.

## Features

- ✅ User authentication (secure, JWT-based)
- ✅ Task creation and management
- ✅ Project organization
- ✅ Mobile-responsive
- ✅ WCAG AA compliant

## Tech Stack

- **Frontend:** React 18, TypeScript, Tailwind CSS
- **Backend:** Node.js 18, Express 4, PostgreSQL 15
- **Testing:** Jest, React Testing Library, Cypress
- **Deployment:** Vercel (frontend), Railway (backend)

## Getting Started

### Prerequisites

- Node.js 18+
- PostgreSQL 15+
- Redis (optional, for sessions)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/taskflow.git
   cd taskflow
   ```

2. Install dependencies:
   ```bash
   npm install
   cd client && npm install
   cd ../server && npm install
   ```

3. Set up environment variables:
   ```bash
   cp server/.env.example server/.env
   # Edit server/.env with your database credentials
   ```

4. Run database migrations:
   ```bash
   cd server
   npm run migrate
   ```

5. Start development servers:
   ```bash
   # Terminal 1: Backend
   cd server && npm run dev

   # Terminal 2: Frontend
   cd client && npm run dev
   ```

6. Open http://localhost:3000

### Testing

```bash
# Unit and integration tests
npm test

# E2E tests
npm run test:e2e

# Test coverage
npm run test:coverage
```

## Architecture

[Include diagram or link to architecture document]

## Spec-Kit Artifacts

All Spec Kit artifacts are in the `/spec-kit/` directory:
- `CONSTITUTION.md`: Project principles and constraints
- `SPECS/`: Detailed specifications
- `PLANS/`: Implementation plans
- `TASKS/`: Task breakdowns
- `CHECKLIST.md`: Progress tracking

## Deployment

[Include deployment instructions]

## License

MIT

## Contact

[Your name/email]
```

---

## Assessment Rubric

### Specifications (25 points)

| Criterion | Exemplary (5) | Proficient (4) | Developing (3) | Needs Work (0-2) |
|-----------|--------------|----------------|----------------|------------------|
| **Clarity** | Unambiguous, precise language | Mostly clear with minor ambiguities | Some unclear sections | Vague, hard to understand |
| **Completeness** | All requirements covered, edge cases addressed | Most requirements covered | Some gaps in coverage | Major gaps |
| **User-Centricity** | Deeply grounded in user needs, validated | User needs considered | Minimal user focus | No user consideration |
| **Testability** | Can write comprehensive tests directly from specs | Can write most tests | Some specifications hard to test | Not testable |
| **Consistency** | Fully consistent across specs, no contradictions | Mostly consistent | Some inconsistencies | Major contradictions |

**Total: /25**

---

### Implementation (25 points)

| Criterion | Exemplary (5) | Proficient (4) | Developing (3) | Needs Work (0-2) |
|-----------|--------------|----------------|----------------|------------------|
| **Functionality** | Fully implements specs, exceeds expectations | Implements all core requirements | Some features incomplete | Minimal functionality |
| **Code Quality** | Clean, well-structured, follows best practices | Good code quality, minor issues | Inconsistent quality | Poor code quality |
| **Testing** | Comprehensive tests, >90% coverage | Good test coverage, >80% | Some tests, 60-80% coverage | Minimal or no tests |
| **Performance** | Meets all performance targets | Meets most targets | Some performance issues | Poor performance |
| **Accessibility** | WCAG AA+ compliance, tested with users | WCAG AA compliance | Partial accessibility | Not accessible |

**Total: /25**

---

### AI Integration (15 points)

| Criterion | Exemplary (5) | Proficient (3-4) | Developing (2) | Needs Work (0-1) |
|-----------|--------------|------------------|----------------|------------------|
| **Effectiveness** | AI significantly accelerated development | AI moderately helpful | AI minimally helpful | AI not used or ineffective |
| **Documentation** | Clear prompts, outputs, and reflection | Documented AI usage | Minimal documentation | No documentation |
| **Analysis** | Thoughtful comparison of with/without AI, lessons learned | Some analysis | Superficial analysis | No analysis |

**Total: /15**

---

### Process & Professionalism (20 points)

| Criterion | Exemplary (5) | Proficient (4) | Developing (3) | Needs Work (0-2) |
|-----------|--------------|----------------|----------------|------------------|
| **Workflow** | Exemplary use of full Spec Kit workflow | Good workflow adherence | Partial workflow use | Minimal workflow |
| **Documentation** | Comprehensive, professional docs | Good documentation | Adequate documentation | Poor or missing docs |
| **Git History** | Clean, meaningful commits | Good commit history | Inconsistent commits | Poor commit history |
| **Presentation** | Polished, portfolio-quality | Professional quality | Adequate presentation | Unprofessional |

**Total: /20**

---

### Advanced/Innovation (15 points)

Choose 1-3 advanced requirements (5 points each):

- [ ] Formal verification (5 pts)
- [ ] Enterprise features (5 pts)
- [ ] Performance optimization with metrics (5 pts)
- [ ] Internationalization (5 pts)
- [ ] Advanced AI (multi-agent, etc.) (5 pts)
- [ ] Research component (5 pts)
- [ ] Open source publication (5 pts)
- [ ] Other innovation (justify) (5 pts)

**Total: /15**

---

### **Grand Total: /100**

**Grading Scale:**
- **90-100:** Distinction (Mastery level)
- **80-89:** Pass with Merit (Strong competence)
- **70-79:** Pass (Competent)
- **Below 70:** Needs revision

---

## Submission Requirements

### What to Submit

1. **Code Repository:**
   - GitHub/GitLab link
   - Public or provide access
   - Include all Spec Kit artifacts in `/spec-kit/` directory

2. **Documentation:**
   - README with setup and usage instructions
   - Architecture overview
   - API documentation (if applicable)

3. **Reflection Document:**
   - What you learned
   - What worked well with Spec Kit
   - What was challenging
   - How you integrated AI
   - What you'd do differently
   - (2-3 pages)

4. **Demo Video:** (Optional but recommended)
   - 5-10 minute walkthrough
   - Show key features
   - Explain architectural decisions
   - Discuss Spec Kit process
   - Upload to YouTube/Vimeo

5. **Presentation Slides:** (Optional)
   - For presenting to class/peers
   - 10-15 slides
   - High-level overview

### Submission Format

```
capstone-submission/
├── README.md (Link to repository and resources)
├── reflection.md (Your reflection document)
├── demo-video.md (Link to video)
├── presentation.pdf (Optional: Slides)
└── assessment-checklist.md (Self-assessment against rubric)
```

### Deadlines

- **Proposal:** [Week 1] (if doing custom project)
- **Mid-Project Check-in:** [Week 3] (optional but recommended)
- **Final Submission:** [Week 6]
- **Presentations:** [Week 7] (optional)

---

## Sample Projects

### Example 1: TaskFlow (Task Management)

**Repository:** [github.com/example/taskflow-capstone](https://github.com/example/taskflow-capstone)

**Highlights:**
- Complete Spec Kit artifact set (constitution, 5 specs, 5 plans, 20+ tasks)
- Full authentication system with JWT
- Task CRUD with project organization
- Accessibility: WCAG AA compliant, tested with NVDA
- AI Integration: 60% of code generated by AI, documented with prompts
- Performance: <2s load time, optimized queries
- Test coverage: 87%

**Spec Kit Process:**
- Constitution defined core principles (speed, accessibility, privacy)
- Specs written before any code
- AI generated initial implementations from specs
- Human validation and refinement
- Continuous spec updates as requirements evolved

**Score:** 94/100 (Distinction)

---

### Example 2: API Doc Generator

**Repository:** [github.com/example/api-doc-gen](https://github.com/example/api-doc-gen)

**Highlights:**
- Parses OpenAPI 3.0 specs
- Interactive "try it out" functionality
- Fast search (<100ms for 500+ endpoints)
- Mobile-responsive, accessible
- Advanced: i18n support (English, Spanish, French)
- Open sourced with 50+ stars

**Spec Kit Process:**
- Used experiment specs to validate approach
- Spike specs to compare rendering libraries
- Full specs for production features
- AI generated 70% of parsing logic
- Continuous improvement specs for enhancements

**Score:** 96/100 (Distinction)

---

## Tips for Success

### 1. Start with the Constitution

**Why:** It guides all other decisions

**How:**
- Spend 1-2 hours defining principles
- Get feedback from peers or mentor
- Refer back to it when making decisions

### 2. Spec First, Code Later

**Why:** Prevents rework and maintains focus

**How:**
- Write specs for all features before implementing
- Review specs with peers
- Only start coding when specs are clear

### 3. Integrate AI Early

**Why:** Maximize productivity gains

**How:**
- Start with simple prompts, refine iteratively
- Document what works and what doesn't
- Use AI for boilerplate, humans for architecture

### 4. Test as You Go

**Why:** Easier than retroactive testing

**How:**
- Write tests alongside implementation
- Run tests frequently (CI/CD)
- Don't merge without tests

### 5. Get Feedback Early and Often

**Why:** Catch issues before they compound

**How:**
- Share specs with peers
- Demo progress weekly
- Ask for code reviews

### 6. Track Your Time

**Why:** Understand where effort goes

**How:**
- Log hours per task
- Compare estimates vs. actuals
- Reflect on efficiency

### 7. Iterate on Specs

**Why:** Specs evolve with understanding

**How:**
- Update specs when requirements change
- Document why changes were made
- Keep specs in sync with code

### 8. Focus on User Value

**Why:** Technical excellence means nothing without user value

**How:**
- Validate with real or simulated users
- Test usability, not just functionality
- Measure success by user outcomes

---

## Frequently Asked Questions

**Q: Can I work in a team?**  
A: Yes, teams of 2-3 are allowed. Clearly document individual contributions.

**Q: Can I use existing code or libraries?**  
A: Yes, using libraries is encouraged. Existing code (yours or others') is okay if properly attributed and you demonstrate Spec Kit process.

**Q: What if I don't finish in time?**  
A: Scope down. It's better to have 3 complete, polished features than 10 half-done features.

**Q: Do I need to deploy to production?**  
A: No, but it's impressive. At minimum, provide clear deployment instructions.

**Q: Can I change my project midway?**  
A: Yes, but document why in your reflection. Use this as a learning opportunity (pivot is a valid outcome).

**Q: How much AI assistance is too much?**  
A: No limit on AI usage. But you must understand and validate all AI-generated code. Human judgment is required.

**Q: What if I can't hit all accessibility targets?**  
A: Document what you attempted and what prevented full compliance. Partial credit for demonstrating effort and understanding.

**Q: Can I use a different workflow than Spec Kit?**  
A: This is a Spec Kit capstone. You must demonstrate Spec Kit workflow. You can augment, but core workflow must be Spec Kit.

---

## Resources

**Spec Kit:**
- [Documentation](https://docs.spec-kit.dev)
- [Examples](https://github.com/spec-kit/examples)
- [Community Forum](https://discuss.spec-kit.dev)

**AI Assistants:**
- GitHub Copilot
- ChatGPT / Claude
- Cursor IDE

**Testing:**
- Jest (JavaScript)
- Pytest (Python)
- JUnit (Java)
- Cypress (E2E)

**Accessibility:**
- [WCAG Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
- [axe DevTools](https://www.deque.com/axe/devtools/)
- [WebAIM](https://webaim.org/)

**Deployment:**
- Vercel (frontend)
- Railway (backend)
- Netlify (static sites)
- Render (full-stack)

---

## Final Thoughts

This capstone is your opportunity to demonstrate everything you've learned about spec-driven development. It's challenging, but you're prepared.

**Remember:**
- Specs guide your work
- AI accelerates implementation
- Users validate success
- Quality matters more than quantity

**Most importantly:**
- Have fun
- Learn from challenges
- Build something you're proud of

**Good luck! You've got this.** 🚀

---

## Navigation

← [Previous: Module 7 Review Quiz](Module-07-Review-Quiz.md)  
↑ [Back to Module 7](../Module-07-Mastery/)  
🏠 [Course Home](../00-Course-Overview.md)
