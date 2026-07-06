# [JIRA-ID] - Agent-Ready User Story: [Brief Description]

<!-- 
INSTRUCTIONS FOR PRODUCT OWNER / DEVELOPER:
- Fill in the sections below to ensure the AI coding agent has enough context to act autonomously.
- Be explicit about constraints and file paths to avoid hallucinations.
- Delete this instruction comment block before saving.
-->

## 1. Context & Objectives
*   **Persona / Role**: As a `[Developer / QA / DevOps]` agent...
*   **Goal**: I want to `[achieve X]`...
*   **Business Value**: So that `[benefit/value Y is realized]`.
*   **Problem Statement**: `[Why is this being done? What is the current broken/missing behavior?]`

## 2. Technical Scope & System Boundary
*   **Target Components**: `[Frontend / Backend / Database / API / CI-CD]`
*   **Target Files (if known)**:
    - `[Relative path to file 1]` (e.g., `src/components/Header.jsx`)
    - `[Relative path to file 2]`
*   **System Dependencies**: `[e.g., Depends on API endpoint /v1/users, or depends on package lodash]`

## 3. Acceptance Criteria (Gherkin Format)
<!-- Write concrete Given/When/Then scenarios. This allows the AI agent to write matching test cases. -->

### Scenario 1: [Name of Scenario]
*   **Given** [Initial system state or context]
*   **When** [The user or system performs an action]
*   **Then** [The expected outcome or state change]

### Scenario 2: [Name of Scenario]
*   **Given** [Context]
*   **When** [Action]
*   **Then** [Outcome]

## 4. Technical Constraints & Design Systems
*   **Do's**:
    - [ ] `[Rule 1: e.g., Use HSL CSS variables for styling]`
    - [ ] `[Rule 2: e.g., Implement unit tests under tests/]`
*   **Don'ts**:
    - [ ] `[Constraint 1: e.g., Do not install any new npm dependencies]`
    - [ ] `[Constraint 2: e.g., Do not modify the database schema]`
*   **Design Tokens/Assets**: `[Links to Figma designs, Tailwind classes to use, or specific styling parameters]`

## 5. Verification & Testing Instructions
*   **Automated Verification**:
    - Run unit tests: `[Command, e.g., npm run test]`
    - Lint check: `[Command, e.g., npm run lint]`
    - Build check: `[Command, e.g., npm run build]`
*   **Manual Verification Steps**:
    1. `[Step 1 to manually verify: e.g., Navigate to /login]`
    2. `[Step 2: e.g., Fill in invalid credentials]`
    3. `[Step 3: e.g., Assert validation message is displayed]`

## 6. References & Attachments
*   **API Schema**: `[Link or inline markdown block showing payload schemas]`
*   **Figma Link**: `[URL to Figma file]`
*   **Related Issues**: `[Epic / Parent Story / Blocking Tickets]`
